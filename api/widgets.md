FORMAT: 1A
HOST: https://pledgeit.org/api-public/widgets

# Pledge It Widget API
A collection of useful endpoints for creating external widgets for Pledge It site content.

**Base URL** `https://pledgeit.org/api-public/widgets`

## Widget Data

### Get a campaign [GET /campaigns/{campaign_slug}]

+ Parameters
    + campaign_slug: `test-campaign` (string) - The unique slug found in the campaign url

+ Response 200 (application/json)

    ```js
    {
        "id": "000000000000000000000000",
        "slug": "test-campaign",
        "name": "A really awesome campaign",
        "image": "https://res.cloudinary.com/pledge-it/image/upload/t_widget/facebook-default",
        "completionDate": "2018-03-29T20:00:00.000Z",
        "status": "active",
        "performanceTotal": 3,
        "amountRaised": "150.00",
        "amountPerMetric": "50.00",
        "contributorCount": 2,
        "url": "http://pledgeit.test/test-campaign",
        "fundraiseUrl": "http://pledgeit.test/test-campaign/fundraise",
        "contributeUrl": "http://pledgeit.test/test-campaign/contribute",
        "performanceMetric": {
            "plural": "touchdowns",
            "singular": "touchdown"
        },
        "performanceEvent": {
            "plural": "games",
            "singular": "game"
        }
    }
    ```

### Get a template [GET /templates/{template_slug}]

+ Parameters
    + template_slug: `test-template` (string) - The unique slug found in the template url

+ Response 200 (application/json)

    ```js
    {
        "id": "5a74c0382e8dc8527bd1561f",
        "slug": "test-template",
        "name": "A really awesome template",
        "image": "https://res.cloudinary.com/pledge-it/image/upload/t_widget/facebook-default",
        "active": true,
        "campaignCount": 12,
        "amountRaised": "1,500.00",
        "url": "http://pledgeit.test/for/test-template"
    }
    ```
