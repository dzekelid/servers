{
  "info": {
    "name": "Etsy Get Server Ping",
    "_postman_id": "1a28ca01-6a1f-443d-9fb8-3d5d57a559e8",
    "description": "Check that the server is alive.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "f7585495-61bf-4aca-bf8e-5df38a2e8b3f",
          "name": "getCountriesCountry",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "countries/:country_id"
              ],
              "variable": [
                {
                  "id": "country_id",
                  "value": "country_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Country by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "857f7624-7153-475d-89fb-31169d4aa5ef"
            }
          ]
        },
        {
          "id": "f881d39e-0959-4d2a-a0fb-6946827b1821",
          "name": "getCountries",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/countries",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all Country."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72b06f68-b246-478c-8326-5d6db8809ce8"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "d240979d-5517-4016-958b-b529dd151bd4",
          "name": "getUsersUserFavoritesListings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all favorite listings for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50f952a7-55b6-4a27-8e7b-d7c206cddeac"
            }
          ]
        },
        {
          "id": "6a082533-f436-451a-8b54-e46d5d03a454",
          "name": "getUsersUserFavoritesListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds a favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5dd10b58-b91b-438a-9061-3983bb61ddcd"
            }
          ]
        },
        {
          "id": "1f83f938-9ba8-4db8-a4f6-78629fbf2450",
          "name": "postUsersUserFavoritesListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "673b341b-c2bc-4a4a-b297-94fb90cf96fd"
            }
          ]
        },
        {
          "id": "4090af1c-b8c7-41a6-9246-568caad2d784",
          "name": "deleteUsersUserFavoritesListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f865179d-caa1-40cc-8e96-c8f80ede4c31"
            }
          ]
        },
        {
          "id": "0750eacd-0242-4195-96e2-61c22f5ab891",
          "name": "getUsersUserFavoritesUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all favorite users for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c7da0d3-4d3f-4bae-ad84-daa62d95b54b"
            }
          ]
        },
        {
          "id": "3400916e-1a1a-4a22-950b-4eb070b8c148",
          "name": "getUsersUserFavoritesUsersTargetUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users/:target_user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "target_user_id",
                  "value": "target_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds a favorite user for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "78ae3ec1-d07c-417a-9f9d-00ad9a4dbf4e"
            }
          ]
        },
        {
          "id": "c881f3f3-9020-4cf7-bf24-04de485732ce",
          "name": "postUsersUserFavoritesUsersTargetUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users/:target_user_id"
              ],
              "variable": [
                {
                  "id": "target_user_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e842a0a-6a1a-4b56-b589-905cbd8a6902"
            }
          ]
        },
        {
          "id": "cfc1832a-9874-46f3-a5b8-164734c26aed",
          "name": "deleteUsersUserFavoritesUsersTargetUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favorites/users/:target_user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "target_user_id",
                  "value": "target_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a favorite listing for a user"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ba02fdd-2dbd-407f-85ff-3ff81dabd625"
            }
          ]
        },
        {
          "id": "0ad874d9-3518-4ad3-9993-7db68fc11a03",
          "name": "getUsersUserRecommendedListings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/recommended_listings"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get recommended listings for an authenticated member. The number of listings returned may not match the specified limit if there is no activity from recommended shops."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a0049d2-2e9b-4c12-8009-0fbc51179961"
            }
          ]
        },
        {
          "id": "c59612d8-1855-4ae9-8c5b-f46cf2226f81",
          "name": "postUsersUserRecommendedListingsRejectsListingS",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/recommended_listings/rejects/:listing_ids"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_ids",
                  "value": "listing_ids",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Registers rejections of recommended listings. Affects future recommended listings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97938b1b-edb1-4674-a124-baf0a1621c52"
            }
          ]
        },
        {
          "id": "ffe2a722-56b1-4950-9ddb-49bab03de3b0",
          "name": "postUsersUserRecommendedListingsViewsListingS",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/recommended_listings/views/:listing_ids"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "listing_ids",
                  "value": "listing_ids",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Register viewings of recommended listings. Affects future recommended listings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "893c9254-14ea-465a-97ff-fd6d1d4ac91c"
            }
          ]
        },
        {
          "id": "88a99c0c-93f1-454c-b940-ad80a837defe",
          "name": "getUsersUserTreasuries",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/treasuries"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user's Treasuries"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67ea9389-3039-4ece-bc7c-f627d7fc1bb4"
            }
          ]
        },
        {
          "id": "02ee5ab7-2748-4215-8025-db464e3494d1",
          "name": "getUsersUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a User by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f61d2e1-85fc-437b-b333-831a30288193"
            }
          ]
        },
        {
          "id": "64bb520e-d814-4b9a-96ac-3c9d80a43628",
          "name": "getUsersUserShops",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/shops"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Shop objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1268f07d-cad2-486b-b695-2eba5c148883"
            }
          ]
        },
        {
          "id": "acc3b8f2-2983-4892-bfdf-1e5bbcaf2ae0",
          "name": "getUsersUserFavoredBy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/favored-by"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of FavoriteUser objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3487f2df-1a07-4940-80c5-501f192e75ca"
            }
          ]
        },
        {
          "id": "401d52b6-dc72-4528-ae70-c81a84c76788",
          "name": "getUsersUserFeedbackAsSubject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-subject"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fcde5077-c4a0-4e4b-80f2-da4bf417acf3"
            }
          ]
        },
        {
          "id": "0958aee0-4a4b-4437-9152-b020a486482e",
          "name": "getUsersUserFeedbackAsAuthor",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-author"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "659dd5ff-adff-424d-98ea-9942e323564b"
            }
          ]
        },
        {
          "id": "99337e5e-7fbe-45eb-935b-f5057753cd1e",
          "name": "getUsersUserFeedbackAsBuyer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-buyer"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "46478e6c-ea37-4fa7-b151-3e0ef4b2dc8c"
            }
          ]
        },
        {
          "id": "e022fbe9-ded6-465c-abc7-19465274d6a2",
          "name": "getUsersUserFeedbackAsSeller",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/feedback/as-seller"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Feedback objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ef10ee10-4376-4700-8a91-c06dbba96eb9"
            }
          ]
        },
        {
          "id": "a7ce9a57-1865-4c6b-b536-6ffd04a403fe",
          "name": "getUsersUserOrders",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/orders"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Order objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0ce98ad3-8df2-4348-944d-8f6176b82206"
            }
          ]
        },
        {
          "id": "b3b5250b-234f-4088-a7b8-91dc123ae768",
          "name": "getUsersUserReceipts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/receipts"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Receipt objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bde0687-d800-4939-876f-5dbe30119e2f"
            }
          ]
        },
        {
          "id": "cd060d1b-4a57-41d2-b654-fef0e4e73647",
          "name": "getUsersUserTransactions",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/transactions"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Transaction objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "745d6487-b73c-4844-b842-333be8501e98"
            }
          ]
        },
        {
          "id": "fcd0c0f4-f1df-49a5-9b89-7dc6083ba92a",
          "name": "getUsersUserCharges",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/charges"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of BillCharge objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8b53f14-1e25-4fc5-922e-4b05526d48a7"
            }
          ]
        },
        {
          "id": "76ee4250-5774-447c-8cc7-2bbecd5bc47c",
          "name": "getUsersUserPayments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/payments"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of BillPayment objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d54b2f04-4267-4a70-acc1-75f24dffbe99"
            }
          ]
        },
        {
          "id": "59953076-e50c-4dbb-863a-1ddeebacbdfc",
          "name": "getUsersUserShippingTemplates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/shipping/templates"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ShippingTemplate objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dbb4b3ec-d074-44c5-94fc-84e557790dbd"
            }
          ]
        },
        {
          "id": "11c45a3f-cba2-4137-b73c-007c0d86b26b",
          "name": "getUsersUserPaymentsTemplates",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/payments/templates"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of PaymentTemplate objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "377efc3d-b85a-4ac9-b8c9-812f561bc376"
            }
          ]
        },
        {
          "id": "f203e858-0c7b-4770-8d48-87d04f2bca7c",
          "name": "getUsersUserAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of UserAddress objects associated to a User."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb6f2d40-79cf-43a1-9403-261753ca89af"
            }
          ]
        },
        {
          "id": "68bbd110-1767-4781-991b-346f55f8b287",
          "name": "postUsersUserAddresses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses"
              ],
              "query": [
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "first_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "second_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "zip",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new UserAddress."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "82110150-7a2c-4ed8-84ca-aa92368c19cc"
            }
          ]
        },
        {
          "id": "05b72264-7ecf-4761-9afa-708fed02622b",
          "name": "postUsersUserAvatar",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/avatar"
              ],
              "query": [
                {
                  "key": "image",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "src",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new user avatar image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd4aee79-9d24-424d-adcd-317f90b4e76d"
            }
          ]
        },
        {
          "id": "c42dc941-1503-4f1d-8e48-e21b800390c7",
          "name": "getUsersUserAvatarSrc",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/avatar/src"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get avatar image source"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8617096-28f3-4af9-9078-7fee8b76535e"
            }
          ]
        },
        {
          "id": "90e176f0-bb61-4e48-892b-353fb97bc086",
          "name": "getUsersUserAddressesUserAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses/:user_address_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "user_address_id",
                  "value": "user_address_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a UserAddress by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "939b63f9-8960-467f-b7c1-ea14775e33c0"
            }
          ]
        },
        {
          "id": "61d10e84-8b8a-47d9-af56-35913f175baa",
          "name": "putUsersUserAddressesUserAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses/:user_address_id"
              ],
              "query": [
                {
                  "key": "city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "first_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "second_line",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "zip",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "user_address_id",
                  "value": "user_address_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a UserAddress with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "42a47dba-acd8-4a5e-8974-7337ba10e820"
            }
          ]
        },
        {
          "id": "32236a47-31e8-48f9-a266-ca9b5eee8bb1",
          "name": "deleteUsersUserAddressesUserAddress",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "users/:user_id/addresses/:user_address_id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "user_address_id",
                  "value": "user_address_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the UserAddress with the given id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbb7e9c0-8379-440a-bbc3-1e5c3b6f605c"
            }
          ]
        }
      ]
    },
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "48178f78-6c49-4055-9348-9cb32bb30b60",
          "name": "getHomepagesPickers",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/homepages/pickers/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedListingPicker in scope active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2d74bfb-8fe1-446d-a335-64bf0e99d1e1"
            }
          ]
        },
        {
          "id": "3d3819bb-75a4-49db-9d0c-597d3d1c5ea2",
          "name": "getHomepagesPickersFeaturedListingPicker",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a FeaturedListingPicker by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "281f7856-8fe9-4a6c-9fca-7c1ec9176303"
            }
          ]
        },
        {
          "id": "78082c73-6c76-480c-81d2-e28147d4af9a",
          "name": "getHomepagesPickersFeaturedListingPickerFeatured",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id/featured"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of FeaturedListing objects associated to a FeaturedListingPicker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e20d9a1f-82c0-4204-a043-85eea5e8c4de"
            }
          ]
        },
        {
          "id": "7f1f756f-d9cc-47cb-8064-5553d20aac7b",
          "name": "getHomepagesPickersFeaturedListingPickerListings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id/listings"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Listing objects associated to a FeaturedListingPicker."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e7f6f65-e94b-4b2e-b6e7-2de5f5e6b601"
            }
          ]
        },
        {
          "id": "3350a785-fc6a-4720-91f4-3ef208abb4ef",
          "name": "getHomepagesPickersFeaturedListingPickerListingsActive",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/pickers/:featured_listing_picker_id/listings/active"
              ],
              "variable": [
                {
                  "id": "featured_listing_picker_id",
                  "value": "featured_listing_picker_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Listing objects associated to a FeaturedListingPicker in scope active."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "da159c4a-c0c6-4647-831b-7b43e04b9054"
            }
          ]
        },
        {
          "id": "5981d82c-64d9-4cbd-9726-2bc90c52cf16",
          "name": "getHomepagesListings",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/homepages/listings/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedListings regardless of Listing state"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a90ebb8-25e6-4f59-b07a-d7ae6d29be05"
            }
          ]
        },
        {
          "id": "8c158842-d8e8-429a-98a0-15c2ff9dba45",
          "name": "getHomepagesListingsActive",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/homepages/listings/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all FeaturedListings that point to active Listings"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3fb55f0-f192-4b57-b418-2c89995275c3"
            }
          ]
        },
        {
          "id": "5debfbb5-e0ad-40d9-9d27-acbcf2d29b51",
          "name": "getHomepagesListingsFeaturedListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/listings/:featured_listing_id"
              ],
              "variable": [
                {
                  "id": "featured_listing_id",
                  "value": "featured_listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a FeaturedListing by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0adbc554-b386-498c-8e6b-ded13255f8ec"
            }
          ]
        },
        {
          "id": "505aaf3c-e5ad-4957-8337-a3944fb53a43",
          "name": "getHomepagesListingsFeaturedListingPicker",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/listings/:featured_listing_id/picker"
              ],
              "variable": [
                {
                  "id": "featured_listing_id",
                  "value": "featured_listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of FeaturedListingPicker objects associated to a FeaturedListing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d1d91672-680c-490c-90fd-d884176b34da"
            }
          ]
        },
        {
          "id": "09a8e7f2-22f8-4582-b53b-b51917e204c0",
          "name": "getHomepagesListingsFeaturedListingListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "homepages/listings/:featured_listing_id/listing"
              ],
              "variable": [
                {
                  "id": "featured_listing_id",
                  "value": "featured_listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of Listing objects associated to a FeaturedListing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2ec3a993-90bd-4740-b9c1-c497198aa010"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "8b7483e8-a07f-4572-9b3b-a8fadf809528",
          "name": "getListingsListingImagesListingImage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images/:listing_image_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                },
                {
                  "id": "listing_image_id",
                  "value": "listing_image_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a ListingImage by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e0396c91-b775-41bb-bc0b-c8355f25db86"
            }
          ]
        },
        {
          "id": "b9139449-b7b4-48b7-9c27-d2e08c8e1c61",
          "name": "deleteListingsListingImagesListingImage",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images/:listing_image_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                },
                {
                  "id": "listing_image_id",
                  "value": "listing_image_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a listing image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c073c86e-b9e9-4e84-826f-beb3959e8b90"
            }
          ]
        },
        {
          "id": "2d53ba57-1817-43eb-bbcc-32a7a1625022",
          "name": "getListingsListingImages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ListingImage objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3af6efbb-5423-41bd-bf98-498238a0b4d1"
            }
          ]
        },
        {
          "id": "215b19c3-2830-46a2-ac52-6f9a7cdc0fe5",
          "name": "postListingsListingImages",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/images"
              ],
              "query": [
                {
                  "key": "image",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Upload a new listing image"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2ff524a-370d-4327-8f0f-5ac5d45bd583"
            }
          ]
        },
        {
          "id": "efd83118-9162-4166-a742-48d4c2528d5e",
          "name": "getListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a Listing by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8876251-137d-4e02-894c-af1ec776d2c6"
            }
          ]
        },
        {
          "id": "4e23bc12-ab77-4955-9949-39bc25be441c",
          "name": "putListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id"
              ],
              "query": [
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "materials",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "price",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "quantity",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "renew",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "shipping_template_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "shop_section_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "tags",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "title",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Updates a Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a2bbd4d-670e-4864-a249-20582757e257"
            }
          ]
        },
        {
          "id": "a47e8126-2304-40ea-a4f1-4dd9a20e8bb1",
          "name": "deleteListingsListing",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e7e5266-a563-437a-95eb-69e28064f0da"
            }
          ]
        },
        {
          "id": "c7d95157-dfdc-4285-81ec-fcad3a5e2620",
          "name": "getListingsListingFavoredBy",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/favored-by"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of FavoriteListing objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81debdab-d70c-4cdd-9c6b-8fa4ee7800f8"
            }
          ]
        },
        {
          "id": "c07a3414-7862-4cd5-9017-a1fd52ce6c05",
          "name": "getListingsListingShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/shipping/info"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ShippingInfo objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb9f1f7e-d834-47ad-9512-cc6a7db91aec"
            }
          ]
        },
        {
          "id": "764c905d-4d15-40df-8ac7-f058ac4be1ca",
          "name": "postListingsListingShippingInfo",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/shipping/info"
              ],
              "query": [
                {
                  "key": "destination_country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "origin_country_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "primary_cost",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "region_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "secondary_cost",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new ShippingInfo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f56615f0-8d2f-4b46-aece-05054fb67afd"
            }
          ]
        },
        {
          "id": "be0e85d0-1856-4cf0-9556-61e9fc7fedbe",
          "name": "getListingsListingPayments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "openapi.etsy.com",
              "path": [
                "v2",
                "private",
                "listings/:listing_id/payments"
              ],
              "variable": [
                {
                  "id": "listing_id",
                  "value": "listing_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a set of ListingPayment objects associated to a Listing."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "651aad68-2637-4669-8a87-6b032a330d5b"
            }
          ]
        },
        {
          "id": "7be234dc-706e-4de2-9edf-e1c5ac1f560f",
          "name": "getListingsActive",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/listings/active",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Finds all active Listing"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0fc5775-b4cf-4026-b987-f68fc27c52b0"
            }
          ]
        },
        {
          "id": "83341586-631a-4bd7-9ef5-b9ee66ca3470",
          "name": "postListings",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/listings?description=%7B%7D&materials=%7B%7D&price=%7B%7D&quantity=%7B%7D&shipping_template_id=%7B%7D&shop_section_id=%7B%7D&tags=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new Listing"
    