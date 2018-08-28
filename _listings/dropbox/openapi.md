swagger: "2.0"
x-collection-name: Dropbox
x-complete: 1
info:
  title: Dropbox Notify Appendix API v1
  description: the-dropbox-notify--is-a-part-of-dropbox-core-ap-with-a-separate-endpoint-for-notification-call-
  termsOfService: https://www.dropbox.com/developers/reference/tos
  contact:
    name: Dropbox
    url: https://www.dropbox.com/developers
  version: 1.0.0
host: api-notify.dropbox.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /shares/{root}/{path}:
    post:
      summary: Creates and returns a shared link to a file or folder.
      description: |-
        Creates and returns a [shared link](https://www.dropbox.com/help/167) to a file or folder.

        Dropbox for Business users can set restrictions on shared links; the `visibility` field indicates what
        (if any) restrictions are set on this particular link. Possible values include:
          * `PUBLIC` - anyone can view
          * `TEAM_ONLY` - only the owner's team can view
          * `PASSWORD` - a password is required
          * `TEAM_AND_PASSWORD` - a combination of `TEAM_ONLY` and `PASSWORD` restrictions
          * `SHARED_FOLDER_ONLY` - only [members](https://www.dropbox.com/help/6636) of the enclosing shared folder can view

        Note that other values may be added at any time.
      operationId: creates-and-returns-a-shared-linkhttpswwwdropboxcomhelp167-to-a-file-or-folderdropbox-for-business-u
      x-api-path-slug: sharesrootpath-post
      parameters:
      - in: formData
        name: locale
        description: Use to specify language settings for user error messages and
          other language specific text
      - in: path
        name: path
        description: The path to the file or folder you want to link to
      - in: path
        name: root
        description: 'Root folder: `auto` - automatically determines the appropriate
          root folder using your apps permissionlevel (recommended); `sandbox` - the
          codename for app folder level; `dropbox` - full dropbox access'
      - in: formData
        name: short_url
        description: When `true` (default), the URL returned will be shortened using
          the Dropbox URL shortener
      responses:
        200:
          description: OK
      tags:
      - Storage
      - Documents
      - Shares
      - Root
      - Path