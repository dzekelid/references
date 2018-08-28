---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Gets all tenancy referencing applications for the caseId provided
  version: 1.0.0
  description: Gets all tenancy referencing applications for the caseid provided.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/printablepropertylist:
    post:
      summary: Generates a printable property list, it is targetless so there is no
        reference to applicants or owners
      description: Generates a printable property list, it is targetless so there
        is no reference to applicants or owners.
      operationId: DocumentGeneration_PrintablePropertyListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationprintablepropertylist-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Printable
      - Property
      - List
      - ""
      - It
      - Is
      - Targetless
      - So
      - There
      - Is
      - "No"
      - Reference
      - To
      - Applicants
      - Owners
  /api/Job:
    get:
      summary: Gets the status for a job given its reference
      description: Gets the status for a job given its reference.
      operationId: Job_GetJobStatusByjobReference
      x-api-path-slug: apijob-get
      parameters:
      - in: query
        name: jobReference
        description: The job reference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Statusa
      - Job
      - Given
      - Its
      - Reference
  /api/progression/lettings/referencetenant:
    post:
      summary: Reference a tenant on a tenant role
      description: Reference a tenant on a tenant role.
      operationId: LettingsProgression_ReferenceTenantByidBytenantPersonIdByreferenceStatusByreferenceTypeBynameBynotes
      x-api-path-slug: apiprogressionlettingsreferencetenant-post
      parameters:
      - in: query
        name: id
        description: The id of the tenant role
      - in: query
        name: name
        description: The id of the person to reference
      - in: query
        name: notes
        description: Notes for the reference
      - in: query
        name: referenceDate
        description: Date of the reference if null today is used
      - in: query
        name: referenceStatus
        description: Whether the tenant has passed referencing or not
      - in: query
        name: referenceType
        description: Date of the reference if null today is used
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tenantPersonId
        description: The id of the person to reference
      responses:
        200:
          description: OK
      tags:
      - Reference
      - Tenant
      - "On"
      - Tenant
      - Role
  /api/progression/lettings/referenceguarantor:
    post:
      summary: Reference a guarantor on a tenant role
      description: Reference a guarantor on a tenant role.
      operationId: LettingsProgression_ReferenceGuarantorByidByguarantorPersonIdByreferenceStatusBynameBynotesByreferen
      x-api-path-slug: apiprogressionlettingsreferenceguarantor-post
      parameters:
      - in: query
        name: guarantorPersonId
        description: The id of the person to reference
      - in: query
        name: id
        description: The id of the tenant role
      - in: query
        name: name
        description: The id of the tenant role
      - in: query
        name: notes
        description: Notes of reference
      - in: query
        name: referenceDate
        description: Date of the reference if null today is used
      - in: query
        name: referenceStatus
        description: Whether the guarantor has passed referencing or not
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reference
      - Guarantor
      - "On"
      - Tenant
      - Role
  /api/progression/lettings/detatchdocumentfromreference:
    post:
      summary: Detatch a document from a reference.
      description: Detatch a document from a reference..
      operationId: LettingsProgression_DetatchDocumentFromReferenceByreferenceIdBydocumentId
      x-api-path-slug: apiprogressionlettingsdetatchdocumentfromreference-post
      parameters:
      - in: query
        name: documentId
        description: The tenant Id
      - in: query
        name: referenceId
        description: The tenant Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Detatch
      - Document
      - From
      - Reference
  /api/people/findbyidentity:
    get:
      summary: Gets the person by an identity reference
      description: Gets the person by an identity reference.
      operationId: People_GetPersonByIdentityByissuerBynameidentifier
      x-api-path-slug: apipeoplefindbyidentity-get
      parameters:
      - in: query
        name: issuer
        description: The issuer of the identity
      - in: query
        name: nameidentifier
        description: The nameidentifier of the identity
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Person
      - By
      - Identity
      - Reference
  /api/tenantreferncing/products:
    get:
      summary: Gets the available products for tenant referencing
      description: Gets the available products for tenant referencing.
      operationId: TenantReferencing_GetProducts
      x-api-path-slug: apitenantreferncingproducts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - Available
      - Productstenant
      - Referencing
  /api/tenantreferncing/case/{tenancyRoleId}:
    get:
      summary: Gets a tenancy referencing case based on the role id supplied
      description: Gets a tenancy referencing case based on the role id supplied.
      operationId: TenantReferencing_GetCaseBytenancyRoleId
      x-api-path-slug: apitenantreferncingcasetenancyroleid-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The id of the tenancy role the case linked to
      responses:
        200:
          description: OK
      tags:
      - S
      - Tenancy
      - Referencing
      - Case
      - Based
      - "On"
      - Role
      - Id
      - Supplied
    post:
      summary: Creates a tenancy referencing case using the role id supplied
      description: Creates a tenancy referencing case using the role id supplied.
      operationId: TenantReferencing_CreateCaseBytenancyRoleId
      x-api-path-slug: apitenantreferncingcasetenancyroleid-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The tenancy id the created case will be linked to
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Tenancy
      - Referencing
      - Case
      - Using
      - Role
      - Id
      - Supplied
  /api/tenantreferncing/applications/{caseId}:
    get:
      summary: Gets all tenancy referencing applications for the caseId provided
      description: Gets all tenancy referencing applications for the caseid provided.
      operationId: TenantReferencing_GetApplicationsBycaseId
      x-api-path-slug: apitenantreferncingapplicationscaseid-get
      parameters:
      - in: path
        name: caseId
        description: The id of the case to get applications from
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - ""
      - Tenancy
      - Referencing
      - Applicationsthe
      - CaseId
      - Provided
  /api/tenantreferncing/addapplication/{caseId}/{tenancyRoleId}/{personId}/{productId}:
    post:
      summary: Creates a tenancy referencing application for a case using the details
        supplied
      description: Creates a tenancy referencing application for a case using the
        details supplied.
      operationId: TenantReferencing_CreateApplicationBycaseIdBytenancyRoleIdBypersonIdByproductId
      x-api-path-slug: apitenantreferncingaddapplicationcaseidtenancyroleidpersonidproductid-post
      parameters:
      - in: path
        name: caseId
        description: The id of the case to add the Application to
      - in: path
        name: personId
        description: The id of the individual the application is for
      - in: path
        name: productId
        description: The id of the product the client has chosen
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The role id of the tenancy the case is linked to
      responses:
        200:
          description: OK
      tags:
      - Creates
      - Tenancy
      - Referencing
      - Applicationa
      - Case
      - Using
      - Details
      - Supplied
  /api/tenantreferncing/addguarantor/{caseId}/{tenancyRoleId}/{personId}:
    post:
      summary: Adds a Guarantor to a tenancy referencing application for a case using
        the details supplied
      description: Adds a guarantor to a tenancy referencing application for a case
        using the details supplied.
      operationId: TenantReferencing_CreateApplicationBycaseIdBytenancyRoleIdBypersonId
      x-api-path-slug: apitenantreferncingaddguarantorcaseidtenancyroleidpersonid-post
      parameters:
      - in: path
        name: caseId
        description: The id of the case to add the Guarantor to
      - in: path
        name: personId
        description: The id of the individual the application is for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The role id of the tenancy the case is linked to
      responses:
        200:
          description: OK
      tags:
      - S
      - Guarantor
      - To
      - Tenancy
      - Referencing
      - Applicationa
      - Case
      - Using
      - Details
      - Supplied
  /api/tenantreferncing/submitcase/{tenancyRoleId}/{caseId}:
    put:
      summary: Submits a tenant referencing case for processing
      description: Submits a tenant referencing case for processing.
      operationId: TenantReferencing_SubmitCaseForReferencingBytenancyRoleIdBycaseId
      x-api-path-slug: apitenantreferncingsubmitcasetenancyroleidcaseid-put
      parameters:
      - in: path
        name: caseId
        description: The id of the case to submit
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: tenancyRoleId
        description: The role id of the tenancy the case is linked to
      responses:
        200:
          description: OK
      tags:
      - Submits
      - Tenant
      - Referencing
      - Caseprocessing
  /api/tenantreferncing/submitapplication/{caseId}:
    put:
      summary: Submits an individual referencing application for processing
      description: Submits an individual referencing application for processing.
      operationId: TenantReferencing_SubmitApplicationForReferencingBycaseId
      x-api-path-slug: apitenantreferncingsubmitapplicationcaseid-put
      parameters:
      - in: path
        name: caseId
        description: The id of the case to submit the application for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Submits
      - Individual
      - Referencing
      - Applicationprocessing
  /api/tenantreferncing/application/{applicationId}/referencingresult:
    get:
      summary: Get the details of an individual application referencing result
      description: Get the details of an individual application referencing result.
      operationId: TenantReferencing_GetApplicationStatusByapplicationId
      x-api-path-slug: apitenantreferncingapplicationapplicationidreferencingresult-get
      parameters:
      - in: path
        name: applicationId
        description: The id of the application to retrieve results for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Individual
      - Application
      - Referencing
      - Result
  /api/coreplatformstate/{stateItemReference}:
    delete:
      summary: Clears a state item.
      description: Clears a state item..
      operationId: CorePlatformState_ClearStateItemBystateItemReference
      x-api-path-slug: apicoreplatformstatestateitemreference-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: stateItemReference
        description: The state item reference
      responses:
        200:
          description: OK
      tags:
      - Clears
      - State
      - Item
  /api/documentgeneration/deletesackcontent/{sackReference}/{envelopereference}:
    get:
      summary: "deletes an envelope from the the content of a sack \r\nDeprecated
        in favour of the DELETE verb"
      description: "Deletes an envelope from the the content of a sack \r\ndeprecated
        in favour of the delete verb."
      operationId: DocumentGeneration_DeleteSackContentDeprecatedBysackReferenceByenvelopereference
      x-api-path-slug: apidocumentgenerationdeletesackcontentsackreferenceenvelopereference-get
      parameters:
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Envelope
      - From
      - The
      - Content
      - Of
      - Sack
      - Deprecated
      - In
      - Favour
      - Of
      - DELETE
      - Verb
  /api/documentgeneration/envelopecontent/{sackReference}/{envelopereference}/{documentreference}:
    delete:
      summary: deletes an document from an envelope
      description: Deletes an document from an envelope.
      operationId: DocumentGeneration_DeleteEnvelopeContentBysackReferenceByenvelopereferenceBydocumentreference
      x-api-path-slug: apidocumentgenerationenvelopecontentsackreferenceenvelopereferencedocumentreference-delete
      parameters:
      - in: path
        name: documentreference
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Document
      - From
      - Envelope
  /api/documentgeneration/printsackcontent/{sackReference}/{envelopereference}:
    get:
      summary: Prints an envelope from a sack
      description: Prints an envelope from a sack.
      operationId: DocumentGeneration_PrintSackContentBysackReferenceByenvelopereference
      x-api-path-slug: apidocumentgenerationprintsackcontentsackreferenceenvelopereference-get
      parameters:
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Prints
      - Envelope
      - From
      - Sack
  /api/documentgeneration/processsackcontent/{sackReference}:
    get:
      summary: processes the content of the sack
      description: Processes the content of the sack.
      operationId: DocumentGeneration_ProcessSackContentBysackReference
      x-api-path-slug: apidocumentgenerationprocesssackcontentsackreference-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Processes
      - Content
      - Of
      - Sack
  /api/documentgeneration/sack/{sackReference}:
    delete:
      summary: deletes an envelope from the the content of a sack
      description: Deletes an envelope from the the content of a sack.
      operationId: DocumentGeneration_DeleteSackBysackReference
      x-api-path-slug: apidocumentgenerationsacksackreference-delete
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Envelope
      - From
      - The
      - Content
      - Of
      - Sack
  /api/documentgeneration/sackcontent/{sackReference}:
    get:
      summary: Returns the detail of the all outstanding sacks
      description: Returns the detail of the all outstanding sacks.
      operationId: DocumentGeneration_GetSackContentBysackReference
      x-api-path-slug: apidocumentgenerationsackcontentsackreference-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Returns
      - Detail
      - Of
      - ""
      - Outstanding
      - Sacks
  /api/documentgeneration/sackcontent/{sackReference}/{envelopereference}:
    delete:
      summary: deletes an envelope from the the content of a sack
      description: Deletes an envelope from the the content of a sack.
      operationId: DocumentGeneration_DeleteSackContentBysackReferenceByenvelopereference
      x-api-path-slug: apidocumentgenerationsackcontentsackreferenceenvelopereference-delete
      parameters:
      - in: path
        name: envelopereference
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Deletes
      - Envelope
      - From
      - The
      - Content
      - Of
      - Sack
  /api/documentgeneration/updateemailsackcontent/{sackReference}:
    post:
      summary: updates the content of a sack
      description: Updates the content of a sack.
      operationId: DocumentGeneration_UpdateEmailSackContentBysackReferenceByemail
      x-api-path-slug: apidocumentgenerationupdateemailsackcontentsackreference-post
      parameters:
      - in: body
        name: email
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Content
      - Of
      - Sack
  /api/documentgeneration/updateprintsackcontent/{sackReference}:
    post:
      summary: updates the content of a sack
      description: Updates the content of a sack.
      operationId: DocumentGeneration_UpdatePrintSackContentBysackReferenceByprint
      x-api-path-slug: apidocumentgenerationupdateprintsackcontentsackreference-post
      parameters:
      - in: body
        name: print
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Content
      - Of
      - Sack
  /api/documentgeneration/updatetextsackcontent/{sackReference}:
    post:
      summary: updates the content of a sack
      description: Updates the content of a sack.
      operationId: DocumentGeneration_UpdateTextSackContentBysackReferenceBytxt
      x-api-path-slug: apidocumentgenerationupdatetextsackcontentsackreference-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: sackReference
      - in: body
        name: txt
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Updates
      - Content
      - Of
      - Sack
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---