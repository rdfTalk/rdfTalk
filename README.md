# rdfTalk

  RDF Virtual Machine or RDF computing platform based on Smalltalk philosophy and design.
  
  Inside of the machine:

  **Every object is a resource** => every VM object has it's own IRI (Internationalized URI) and can be accessible and changeable from anywhere on the internet if access is granted.
  
  **Every resource is an object** => every resource can be instantiated as an object in VM, fetched, cached, manipulated, updated remotely, uploaded back.

  **Conclusion**: Messaging between resources making the whole server implementation transparent to user/devs enabling them to focus only on higher levels of RDF computing. It brings a concept: *Internet as an image*.

  Computing with RDFTalk implemented becomes:
  * simple (as Smalltalk), 
  * open,
  * reflective and
  * distributed

## necessary steps

  1. add support for RDF into Smalltalk
  2. make Smalltalk VM to be queryable and updatable as an RDF graph (also from outside of the VM)
  3. ontology for messaging between Resources: definitions of methods, message protocols, transportation means, context.
  4. implement RDF messaging in other SemWeb frameworks and languages

## other thoughts

  * Since Pharo is a whole enviromnent I'm thinking about an UI rendering according to UI definition in RDF data
  * rdfTalk + Semantic Desktop

## status

  * learning Smalltalk (Pharo/Moose), PetitParser and RDF
  * developing full IRI support (RFC3986 and RFC3987)
  * developing RDF library:
    * RDF environment for scoping of prefix and term maps
    * named/unnamed graphs
    * graph stores: in memory, file store, sparql endpoint, ldp, ...)
    * parsers and serializers:
      * RDF/XML
      * N3/Turtle
      * JSON/JSON-LD
      * SPARQL/SPIN
    * SPARQL endpoint/client
    * LDP server/client
    * ...
    * inferencing

### Resources

  * discussion with @svenvc about ZnUrl: https://github.com/svenvc/zinc/issues/14
  * old RDF support (Rikaiko) info http://esug.org/wiki/pier/Promotion/SummerTalk/SummerTalk2006#198216748 and its repo http://www.squeaksource.com/@R3-GqJt9eke6ntIN/ysj_M_RE
  * RDF Virtual Machine http://neno.lanl.gov/Blog/Entries/2008/3/5_The_RDF_Virtual_Machine.html
