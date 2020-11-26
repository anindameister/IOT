# What’s difference between The Internet and The Web ?

- The Internet is a global network of networks while the Web, also referred formally as World Wide Web (www) is collection of information which is accessed via the Internet. 
- Another way to look at this difference is; the Internet is infrastructure while the Web is service on top of that infrastructure.
- Alternatively, the Internet can be viewed as a big book-store while the Web can be viewed as collection of books on that store. 
- At a high level, we can even think of the Internet as hardware and the Web as software!

# Some Recap
## uri=url+urn=iri

- these are the types of resources
- we can share or get the resources between computers on the web or internet
- we interact with the resources in regards to certain rules/ protocols like http;coap
- these http, coap provides verbs such as GET,POST,PUT,DELETE and more. These are the ways that we interact with the resources
- these verbs are registered at IANA
- even if the contents are information resource, we get the representation of the resource
- we can negotiate for the representation of resource by maybe mentioning the ACCEPT(the HTTP header) type or ACCEPT language
- we can negotiate on the contentType along with ACCEPT, eg:ACCEPT ttl
- contentType=mediaType+characterEncoding
- Eg: of above(contentType) is text/html+utf-8(charSet or encoding)
- WebApis can be interacted using xml or json docs
- IOT / WOT: almost same as internet/web
- IOT protocol: COAP
- Coap is binarification of http
- Coap is a req, res interaction b/w client and server
- Coap gives a way to encode different verbs(GET,PUT,POST....) with few bytes
- MQTT: publish/subscribe type of interaction protocol
- MQTT: topicNames and filter, QoS(quality of service)
- WebArchitectural styles like REST & HATEOAS
- level 1:designing the http verbs
- level 2:interaction with the resources with the http verbs that are designed in level 1
- level 3: we receive the resource(which is actually a representation of resource). Now within this resource represntation, with webLinking, we're guided to the direction of what needs to be done next.
- CoRE(Constrained RESTful Environments )The CoRE Link Format is carried as a payload and is assigned an Internet media type. 

- payload: In computing and telecommunications, the payload is the part of transmitted data that is the actual intended message. 
- Headers and metadata are sent only to enable payload delivery. 
- In the context of a computer virus or worm, the payload is the portion of the malware which performs malicious action.

- A well-known relative URI "/. well-known/core" is defined as a default entry-point for requesting the list of links about resources hosted by a server, 
- and thus performing CoRE Resource Discovery.

![certificate content](https://github.com/anindameister/IOT/blob/master/snaps/34.PNG)

- the above are hypermedia links.
- so I follow the link of the "next" and go to the next page
- again, I do "InspectSource" and go to network tab, followed by choosing the contributor and going to the header to view source

![certificate content](https://github.com/anindameister/IOT/blob/master/snaps/35.PNG)

- Now we have 4 more links

![certificate content](https://github.com/anindameister/IOT/blob/master/snaps/36.PNG)

- the below is just the IANA defined skeleton

![certificate content](https://github.com/anindameister/IOT/blob/master/snaps/37.PNG)

- following the skeleton
- we have a linkTarget, then the type of relation, some attribute
- later we have a newTarget and so on
- anotherTarger and so on
- anchor: means that the relation is not between the current resource and the other target, but it's between the anchor and the other target 
- now the complete list of relations and the complete list of authorised attributes is in the IANA page
- google: iana link relations. we have about,last, next
- link attributes iana.org/protocol