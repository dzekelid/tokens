swagger: "2.0"
x-collection-name: AWS Route 53
x-complete: 1
info:
  title: AWS Route 53 API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2013-04-01/hostedzone/Id/authorizevpcassociation&amp;maxresults=MaxResults?nexttoken=NextToken:
    get:
      summary: List V P C Association Authorizations
      description: 'Gets a list of the VPCs that were created by other accounts and
        that can be associated with a specified hosted zone because you''ve submitted
        one or more CreateVPCAssociationAuthorization requests. Send a GET request
        to the /2013-04-01/hostedzone/hosted zone ID/authorizevpcassociation resource.
        The response to this request includes a VPCs element with a VPC child element
        for each VPC that can be associated with the hosted zone.Amazon Route 53 returns
        up to 50 VPCs per page. To return fewer VPCs per page, include the MaxResults
        parameter:             /2013-04-01/hostedzone/hosted zone ID/authorizevpcassociation?MaxItems=VPCs
        per page                     If the response includes a NextToken element,
        there are more VPCs to list. To get the next page of VPCs, submit another
        ListVPCAssociationAuthorizations request, and include the value of the NextToken
        element from the response in the NextToken request parameter:            /2013-04-01/hostedzone/hosted
        zone ID/authorizevpcassociation?MaxItems=VPCs per page&amp;NextToken='
      operationId: listvpcassociationauthorizations
      x-api-path-slug: 20130401hostedzoneidauthorizevpcassociationampmaxresultsmaxresultsnexttokennexttoken-get
      parameters:
      - in: path
        name: Id
        description: The ID of the hosted zone for which you want a list of VPCs that
          can be associated with the hosted zone
        type: string
      responses:
        200:
          description: OK
      tags:
      - VPC