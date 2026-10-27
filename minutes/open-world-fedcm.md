# FedCM

Open-World Social Sign-in with Decentralized FedCM
* https://www.w3.org/events/meetings/4690848b-ef1b-4c32-85e0-467632e66300/

## Present
* Darius (session chair)
* Sam Goto (SG)
* Evan Prodromou (EP) https://socialwebfoundation.org/ (scribe)
* Tantek Çelik (TÇ) https://tantek.com/ (scribe)
* Manu Sporny (MS) 
* Dmitri Z (DZ)
* Bumblefudge
* Aram
* Emelia (ES)
* Heather
* Brian from Bluesky
* elf Pavlik (Solid/LWS)
* ...


## Handle Problem

- ATProto: use own handle to log into web sites

    - SIFA is an example, LinkedIn of ATProto

    - Login with ATProto username

    - "Open World Federation"

    - Users have to remember their handles to verify


- IndieWeb: Webmention.io

    - can sign in with your own domain


- LWS/SoLiD

    - Knowing your identity provider

    - Every app will do it themselves

    - Inconsistency


- Mastodon API/ActivityPub

    - Select your server to go to the IDP


- Example: log in with Google to Pinterest

    - "closed world"


- Similar to SAML

- Another example: email verification protocol

## Work in Progress

## Proposal Handle Verification 

- Handle verification

- Example: leaflet.pub

    - "Sign in with atmosphere" button

    - RP can suggest identity providers

    - User signs in with handle


- Happy path:

    - Bootstrapped from previous sessions


- Happy path

    - Visited the IdP which pushes the identity onto the 


## Open Discussion

- Do we have a shared problem?

    - Yes


- Is this the right UI?

    - EP: concerns for me are that we have a similar interface to OpenID 1.0, which means we have the same vulnerabilities of OpenID

    - EP: The big improvement is that the browser remembers your ID

    - ES: Adding in the handle is the worst case - normally the person interacting with FedCM will have interacted with their IdP at least once, and therefore had the IdP request to register. But we need to handle the case where that's not so.

    - John: iNames -> CloudNames -> dids (!)

    - Probably a good thing, keeps coming around


- DZ: Big props, biggest problem!

- TÇ: not trauma, experience!

    - was also there for the OpenID experience 20+ years ago, we have iterated and evolved approaches since

    - [rel=me auth](https://indieweb.org/RelMeAuth), then IndieAuth

    - IndieAuth published as a NOTE at the W3C Social Web WG (https://www.w3.org/TR/indieauth/), maintained as living specification: https://indieauth.spec.indieweb.org/ and portions incorporated into IETF specs

    - [PKCE](https://www.rfc-editor.org/info/rfc7636/)

    - UX has improved with iteration and evolution

    - No [NASCAR UIs](https://indieweb.org/NASCAR_problem)!

    - ES: We have provisions for a fallback IdP list so there's some NASCAR, but you can still type your handle and jump directly to your IdP, but this avoids the "thousand little icons" problem of OpenID 1.0


- MS: This is a problem, we should keep working on it

    - MS: UIs look close to credential selectors for digital wallets

    - MS: DC API, other agentic ack screens (?)


- SG: more of a solution problem than a problem problem!

    - SG: adjacent to FedCM UI, which is focused on login

    - SG: FedCM leans towards centralisation

    - ES / SG: So work has been happening to make sure we can support decentralized communties equally with features. That's the IdP Registration work. Blog at: https://decentralizing-fedcm.leaflet.pub/ 


- Bumblefudge: bengo made FedCM4VP
    
- Aram: this seems Google focused, worried about focus on UI

    - ES: open to UI changes, just contact me.




(Evan departed, Tantek scribing a bit)


- Elf: need to figure out different approaches, what are distinct problems

    https://www.w3.org/TR/threat-modeling-guide/#a12-data-flow-diagram-for-minimalist-web-threat-model


    https://github.com/w3c-cg/threat-modeling/issues


- Heather: would be ironic if we identified a centralized group to do decentralized work. FedID CG would be a good place

- ES: have shown up to a lot of meetings, Solid, OWS, have talked with aaronpk for IndieAuth, Brian for atprotocol, have tried to talk to people for activitypub
- ES: if you want someone to come to your group and talk about FedCM and how it fits with your ecosystem, I'm happy to help

- ??? Isn't Paskeys the answer? Sounds like we already have a solution to this problem.

(problems with Zoom)

There was a conversation about passkeys not quite being the answer, since passkeys are bound to the origin that they were created on. FedCM is cross-origins.

- ??? domain, prove yourself with passkey.
- keys you issue yourself

- Aram: passkeys are great for a lot of reasons, also have same problems as a lot of PKI, people fear losing private key and losing account access.
- Aram: as an employee of a company with users over 50, introducing system without a fallback they can rely on is difficult to pitch. it has not caught on in the way a lot of its supporters have hoped

- DZ: passkeys have limitations, bound to one domain. deeply wish we could use them across domains

- Emelia: when you are doing FedCM login flow, you can still use passkey in that flow with your IdP, same with your password manager, since we're just opening a managed popup with your IdP's login URL.

- Brian from Bluesky: re: where should we meet, within the atproto ecosystem, would be helpful if there were one place to funnel the conversation. I don't have a proposal for where that venue should be. Will be at IETF in a few weeks.

    - ES, In chat: For AT Protocol, I know of a few of the groups, but they can always reach out and invite me to their meetings.


- Darius: followup conversation at IETF would be useful

- Sam: I'll be here all week, have been working with people this week, find any of us, pick our brains, try to shape our goals as much as you can. Would love to chat about things. Intersection with credentials, passkeys, other verification. Also a phone number verification breakout coming up. stop by any time. I will be at IETF.

- Darius: we are at time, thank you everyone for coming out and having this discussion. Can find Sam and other folks all week. Continue conversations in hallways

- Emelia: FedCM WG/CG meeting on Thursday: https://www.w3.org/events/meetings/64b54806-62fd-44fc-a3b0-345706c0a184/


