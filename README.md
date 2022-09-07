# DMP Common Standard Ontology

To make it work with our parser in an engine-backend, we had to changed the following things from the [dsco](https://github.com/RDA-DMP-Common/RDA-DMP-Common-Standard/blob/master/ontologies/core/dcso.4.0.0.ttl):

1. Extend the rdfs:domain with the following list for `dcso:identifier` and `dcso:identifierType`:
- `dcso:ContactId`
- `dcso:ContributorId`
- `dcso:DMPId`
- `dcso:DatasetId`
- `dcso:FunderId`
- `dcso:GrantId`
- `dcso:MetadataStandardId`

2. Delete the relation `dcso:hasSecurityPrivacy` due to the absence of fields in the OWL

3. Embed directly the fields of `foaf:mbox` and `foaf:name`

