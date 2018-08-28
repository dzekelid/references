swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/builds/artifacts/{ref_name}/download:
    get:
      summary: Get Projects Builds Artifacts Ref Name Download
      description: Get projects builds artifacts ref name download.
      operationId: getV3ProjectsIdBuildsArtifactsRefNameDownload
      x-api-path-slug: v3projectsidbuildsartifactsref-namedownload-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: query
        name: job
        description: The name for the build
      - in: path
        name: ref_name
        description: The ref from repository
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Builds
      - Artifacts
      - Ref
      - Name
      - Download
  /v3/projects/{id}/(ref/{ref}/)trigger/builds:
    post:
      summary: Post Projects (ref Ref )trigger Builds
      description: Post projects (ref ref )trigger builds.
      operationId: postV3ProjectsId(refRef)triggerBuilds
      x-api-path-slug: v3projectsidrefreftriggerbuilds-post
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: ref
        description: The commit sha or name of a branch or tag
      - in: formData
        name: token
        description: The unique token of trigger
      responses:
        200:
          description: OK
      tags:
      - Projects
      - (ref
      - Ref
      - )trigger
      - Builds