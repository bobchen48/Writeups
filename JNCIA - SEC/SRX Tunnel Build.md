# SRX Route-based VPN Tunnel Building (Conceptual) #

One of the crucial skill learned in JNCIA - SEC was the anatomy of SRX VPN Tunnel. VPN Tunnel sounds cool when it works right? So why not learn the parts that work together to create the VPN!

I remember when I first encountered a VPN configuration. It was 30+ lines of configuration that left my minds blown. Thanks to JNCIA - SEC however, I learned that those 30 lines of configuration can be broken down into a series of steps that work together to build the VPN. But instead of just throwing a ton of commands here, I will explain the conceptual idea behind a VPN Build, specifically _Route-Based VPN_. The steps to build a SRX Route-based VPN are as follows:

## Creating a Secure Tunnel, Security Zones, and Routes ##
>[!NOTE]
>For the two peer to establish a secure tunnel, they will need the necessary interface, security zones and routes configured that will allow them to exchange information

1. **Configure secure tunnel interface**: A secure tunnel interface (st#) is an internal interface that is used by route-based VPNs to route cleartext traffic to an IPsec VPN tunnel.
  
2. **Configure security zone**: We need to identify/define zone that the secure tunnel will reside in.

3. **Configure Route to the secure tunnel**: Route VPN Tunnel via st (st#)

## Phase 1 (IKE - Internet Key Exchange) ##
>[!NOTE]
>IKE Phase 1 is the first Phase of IKE tunnel negotiation process. This phase is used to establish a secure, authenticated channel between the 2 IKE peers. This security channel, also known as IKE Security Association (SA), is then used to securely exchange information and negotiate the IPSec Security Associations (SAs) in Phase 2

4. **Configure Phase 1 (IKE Proposal):**
     - Authentication method
     - Authentication Algorithm (i.e MD5, SHA1, SHA2 etc)
     - Encryption Algorithm (AES is typically the standard encryption algorithm used)
     - Diffie Hellman Group
     - Lifetime
       
5. **Configure IKE Policy:**
     - Mode (Main or Aggressive)
     - Pre-shared Key
     - Name of IKE Proposal (Step 4) to use
       
6. **Configure IKE Gateway**
     - What IKE Policy to use
     - Remote Gateway Address
     - External Interface

## Phase 2 - IPSec ##
>[!NOTE]
>After a secure channel has been established between the two peers in phase 1, phase 2 focuses on Security Associations (SA) negotiation for encrypting and authenticating the actual data traffic exchanged between the two peers

7. **Configure Phase 2 (IPSec Proposal)**
     - Security (ESP/AH)
     - Authentication Algorithm
     - Encryption Algorithm (if using ESP)
     - Lifetime
       
8. **Configure IPSec Policy**
     - Perfect Forward Secrecy (DH Group)
     - IPsec Proposal to be used

9. **Configure IPSec VPN**
     - Gateway
     - IPSec Policy to use
     - Bind to st# interface configured
       
## Security Policy ##
>[!NOTE]
>Now that Phase 1 and Phase 2 have been configured, we need the necessary security policy that permits traffic between Trust zone to the “VPN zone” and from “VPN zone” to the Trust Zone to permit traffic through the tunnel.

10. **Configure security policies**
     - Match Criteria 1
       - source-address Host1-Net
       - destination-address: Host2-Net
       - application any
     - Match Criteria 2
       - source-address Host2-Net
       - destination-address: Host1-Net
       - application any
## External Reference ##
[Route-Based IPSec VPN - Juniper Documentation](https://www.juniper.net/documentation/us/en/software/junos/vpn-ipsec/topics/topic-map/security-route-based-ipsec-vpns.html)



