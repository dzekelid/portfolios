---
swagger: "2.0"
x-collection-name: AWS Service Catalog
x-complete: 0
info:
  title: AWS Service Catalog API Update Portfolio
  version: 1.0.0
  description: Updates the specified portfolio's details.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=AcceptPortfolioShare:
    get:
      summary: Accept Portfolio Share
      description: Accepts an offer to share a portfolio.
      operationId: acceptPortfolioShare
      x-api-path-slug: actionacceptportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=AssociatePrincipalWithPortfolio:
    get:
      summary: Associate Principal With Portfolio
      description: Associates the specified principal ARN with the specified portfolio.
      operationId: associatePrincipalWithPortfolio
      x-api-path-slug: actionassociateprincipalwithportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: PrincipalARN
        description: The ARN representing the principal (IAM user, role, or group)
        type: string
      - in: query
        name: PrincipalType
        description: The principal type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=AssociateProductWithPortfolio:
    get:
      summary: Associate Product With Portfolio
      description: Associates a product with a portfolio.
      operationId: associateProductWithPortfolio
      x-api-path-slug: actionassociateproductwithportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      - in: query
        name: SourcePortfolioId
        description: The identifier of the source portfolio to use with this association
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=CreatePortfolio:
    get:
      summary: Create Portfolio
      description: Creates a new portfolio.
      operationId: createPortfolio
      x-api-path-slug: actioncreateportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Description
        description: The text description of the portfolio
        type: string
      - in: query
        name: DisplayName
        description: The name to use for display purposes
        type: string
      - in: query
        name: IdempotencyToken
        description: A token to disambiguate duplicate requests
        type: string
      - in: query
        name: ProviderName
        description: The name of the portfolio provider
        type: string
      - in: query
        name: Tags
        description: Tags to associate with the new portfolio
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=CreatePortfolioShare:
    get:
      summary: Create Portfolio Share
      description: Creates a new portfolio share.
      operationId: createPortfolioShare
      x-api-path-slug: actioncreateportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccountId
        description: The account ID with which to share the portfolio
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DeletePortfolio:
    get:
      summary: Delete Portfolio
      description: Deletes the specified portfolio.
      operationId: deletePortfolio
      x-api-path-slug: actiondeleteportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the portfolio for the delete request
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DeletePortfolioShare:
    get:
      summary: Delete Portfolio Share
      description: Deletes the specified portfolio share.
      operationId: deletePortfolioShare
      x-api-path-slug: actiondeleteportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AccountId
        description: The account ID associated with the share to delete
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DescribePortfolio:
    get:
      summary: Describe Portfolio
      description: |-
        Retrieves detailed information and any tags associated with the specified
                 portfolio.
      operationId: describePortfolio
      x-api-path-slug: actiondescribeportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: Id
        description: The identifier of the portfolio for which to retrieve information
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DisassociatePrincipalFromPortfolio:
    get:
      summary: Disassociate Principal From Portfolio
      description: |-
        Disassociates a previously associated principal ARN from a specified
                 portfolio.
      operationId: disassociatePrincipalFromPortfolio
      x-api-path-slug: actiondisassociateprincipalfromportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: PrincipalARN
        description: The ARN representing the principal (IAM user, role, or group)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=DisassociateProductFromPortfolio:
    get:
      summary: Disassociate Product From Portfolio
      description: Disassociates the specified product from the specified portfolio.
      operationId: disassociateProductFromPortfolio
      x-api-path-slug: actiondisassociateproductfromportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListAcceptedPortfolioShares:
    get:
      summary: List Accepted Portfolio Shares
      description: |-
        Lists details of all portfolios for which sharing was accepted by this
                 account.
      operationId: listAcceptedPortfolioShares
      x-api-path-slug: actionlistacceptedportfolioshares-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListConstraintsForPortfolio:
    get:
      summary: List Constraints For Portfolio
      description: |-
        Retrieves detailed constraint information for the specified portfolio and
                 product.
      operationId: listConstraintsForPortfolio
      x-api-path-slug: actionlistconstraintsforportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListPortfolioAccess:
    get:
      summary: List Portfolio Access
      description: |-
        Lists the account IDs that have been authorized sharing of the specified
                 portfolio.
      operationId: listPortfolioAccess
      x-api-path-slug: actionlistportfolioaccess-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListPortfolios:
    get:
      summary: List Portfolios
      description: Lists all portfolios in the catalog.
      operationId: listPortfolios
      x-api-path-slug: actionlistportfolios-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListPortfoliosForProduct:
    get:
      summary: List Portfolios For Product
      description: Lists all portfolios that the specified product is associated with.
      operationId: listPortfoliosForProduct
      x-api-path-slug: actionlistportfoliosforproduct-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: ProductId
        description: The product identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=ListPrincipalsForPortfolio:
    get:
      summary: List Principals For Portfolio
      description: Lists all principal ARNs associated with the specified portfolio.
      operationId: listPrincipalsForPortfolio
      x-api-path-slug: actionlistprincipalsforportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PageSize
        description: The maximum number of items to return in the results
        type: string
      - in: query
        name: PageToken
        description: The page token of the first page retrieved
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=RejectPortfolioShare:
    get:
      summary: Reject Portfolio Share
      description: Rejects an offer to share a portfolio.
      operationId: rejectPortfolioShare
      x-api-path-slug: actionrejectportfolioshare-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: PortfolioId
        description: The portfolio identifier
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
  /?Action=UpdatePortfolio:
    get:
      summary: Update Portfolio
      description: Updates the specified portfolio's details.
      operationId: updatePortfolio
      x-api-path-slug: actionupdateportfolio-get
      parameters:
      - in: query
        name: AcceptLanguage
        description: The language code to use for this operation
        type: string
      - in: query
        name: AddTags
        description: Tags to add to the existing list of tags associated with the
          portfolio
        type: string
      - in: query
        name: Description
        description: The updated text description of the portfolio
        type: string
      - in: query
        name: DisplayName
        description: The name to use for display purposes
        type: string
      - in: query
        name: Id
        description: The identifier of the portfolio for the update request
        type: string
      - in: query
        name: ProviderName
        description: The updated name of the portfolio provider
        type: string
      - in: query
        name: RemoveTags
        description: Tags to remove from the existing list of tags associated with
          the         portfolio
        type: string
      responses:
        200:
          description: OK
      tags:
      - Portfolios
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