{
  "info": {
    "name": "Etsy Get Server Epoch",
    "_postman_id": "a06acb8e-1cd9-47ed-b3dc-e29a99481fc4",
    "description": "Get server time, in epoch seconds notation.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Countries",
      "item": [
        {
          "id": "da7d69c4-35fa-46a1-9d5b-a57bc8077db6",
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
              "id": "792f5125-e3dd-475c-ae4d-fbdeb2016cb2"
            }
          ]
        },
        {
          "id": "54325d07-2c94-48db-9237-06072e4f917a",
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
              "id": "71bd264b-81ef-43ef-a5b3-faf00721ef6f"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "be717d2f-9126-4902-ac14-0e79bd30cc59",
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
              "id": "09252a61-3537-4494-805b-5500fc31a572"
            }
          ]
        },
        {
          "id": "939b68c4-cdee-4e7b-ba17-135104366a30",
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
              "id": "57fc4f66-90b9-4f16-9243-dbdd02972951"
            }
          ]
        },
        {
          "id": "fcc5c2bf-acd8-45cd-8d65-b1fa616a606c",
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
              "id": "f284dfa7-446d-4fe1-a1f1-d698eb72e633"
            }
          ]
        },
        {
          "id": "17faaac6-f5a4-4d6b-aa95-e53c2b038e2e",
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
              "id": "e98f70ed-6eb4-4da2-b9bd-7eb945327b91"
            }
          ]
        },
        {
          "id": "31b6bf9e-5d6a-4629-8ebc-8492d225b926",
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
              "id": "ce0024cb-f728-403c-a6a7-70ba2e96adc9"
            }
          ]
        },
        {
          "id": "943a4bf1-34c7-49cc-8a38-41cdabcb0cfd",
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
              "id": "6a1473fc-383a-4052-a6d2-9ed976d79bf8"
            }
          ]
        },
        {
          "id": "1b21f868-053b-4ece-b32c-6c5c27ad7ffd",
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
              "id": "c1563a25-796b-4789-94e4-dfd4761afec1"
            }
          ]
        },
        {
          "id": "ef1cd4c2-b56a-4f62-95bd-a7276f0720ea",
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
              "id": "015f2ac4-c8c0-4d26-afe1-40d0c4494d41"
            }
          ]
        },
        {
          "id": "cf0f765c-547a-497d-91ba-bf4653058667",
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
              "id": "9f2cc5c4-4d74-4549-8c94-6e472d84716e"
            }
          ]
        },
        {
          "id": "6ef89c82-e806-4e6d-bc7a-34b3806778c4",
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
              "id": "48ddfd01-25df-4f7e-9e5c-55c972c585db"
            }
          ]
        },
        {
          "id": "14cfd9c5-51e0-4fc6-988c-88e1d4c5cdd3",
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
              "id": "a327ab84-078a-41c2-90fc-8abbe9c9a816"
            }
          ]
        },
        {
          "id": "b1a00daf-4a6b-4366-bac4-95ec77d013db",
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
              "id": "0e52b4a9-0555-4fec-8da3-73c972128425"
            }
          ]
        },
        {
          "id": "eb17d444-35fd-4ce6-81de-b9e70d47b237",
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
              "id": "77a7c052-a156-4c5a-85f2-faf92e21ceae"
            }
          ]
        },
        {
          "id": "d2275951-a11e-4843-b188-afe910894542",
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
              "id": "ed4b6c3e-1d3d-4580-993e-80e1674869ba"
            }
          ]
        },
        {
          "id": "0b0a15a3-9ea2-46a2-89ee-422127d6f1c1",
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
              "id": "40c01d0c-6413-4633-861f-22e9c49f2845"
            }
          ]
        },
        {
          "id": "5f5cdeec-0ef1-4c43-9423-8c199ba8c84d",
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
              "id": "ccf734cc-6abc-4616-8998-9bec1d551e94"
            }
          ]
        },
        {
          "id": "effecbd4-4015-4806-a96f-3238e75bb7c0",
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
              "id": "e121c251-1caa-44f7-90c2-6aa14233348b"
            }
          ]
        },
        {
          "id": "971adbf7-1afd-409f-b1da-6739c1421fc3",
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
              "id": "8a7a43b9-b33b-4693-a83e-5e077d4b4553"
            }
          ]
        },
        {
          "id": "3ea2cb33-edf4-41af-ac79-f7fbd21c1437",
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
              "id": "ae2c36f0-6940-4afc-9751-f36c052a26bb"
            }
          ]
        },
        {
          "id": "f1ff1082-a47f-4a81-91c7-4ef9054d25c6",
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
              "id": "9b48a378-b90e-44c5-93f7-d7b57dce9149"
            }
          ]
        },
        {
          "id": "73bb472b-ee58-43a9-b2f0-e891e96934d8",
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
              "id": "d3b7a07c-6265-49c7-b956-641bac632b1f"
            }
          ]
        },
        {
          "id": "4f41feba-776f-4c76-ba08-21634bde6af5",
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
              "id": "aee0c8a2-da86-4086-82f5-d57afffc1e4b"
            }
          ]
        },
        {
          "id": "4b5768e2-a327-4f70-b21b-becb888b448e",
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
              "id": "4e9b43f3-00e5-4f72-a1ab-b38ec9712aa2"
            }
          ]
        },
        {
          "id": "be02edef-8dc6-44e7-b707-06e1cbccaf1f",
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
              "id": "c0028549-6dc6-43ad-b301-cdda1bbc7166"
            }
          ]
        },
        {
          "id": "87411f15-439c-4b09-9d38-18ba98b93a0b",
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
              "id": "d4d43522-2000-49c6-afef-1d3247a400ba"
            }
          ]
        },
        {
          "id": "57835718-36a7-4dcd-bc80-ffe6efebc8d4",
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
              "id": "46307c3a-2a00-4098-aed1-25f571d49eb4"
            }
          ]
        },
        {
          "id": "6cecc2f5-d003-46ff-9ab6-36ff80749b8c",
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
              "id": "4ccd7de2-ae02-4b80-b1c3-02598e834afe"
            }
          ]
        },
        {
          "id": "576b347c-1814-44db-918e-329c7416c4b9",
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
              "id": "200f0f10-f68f-432d-b9e5-1e94b2b6c0b3"
            }
          ]
        },
        {
          "id": "3a01bec8-672b-49d2-944a-5adbf546e9ef",
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
              "id": "a9cfb29a-093f-444a-8416-c6f354e2e196"
            }
          ]
        },
        {
          "id": "fde84d95-bbf0-4899-a686-d4c1ff0ea047",
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
              "id": "627c937a-a4d5-422a-b414-86de09f2890e"
            }
          ]
        },
        {
          "id": "a65e86a2-a717-4169-a994-177ce32a5b0a",
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
              "id": "a5a59fa2-ca14-4ec9-bf2d-d8b031a57fea"
            }
          ]
        },
        {
          "id": "c3ec580b-1051-4433-a448-f0569255a360",
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
              "id": "a9adf367-2aad-41e5-b0fa-aac3d94096cf"
            }
          ]
        },
        {
          "id": "b1759a34-f917-4fcb-ba7d-28100d9a9d66",
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
              "id": "40c8e03f-cd2b-4f71-9985-96a715a1a2c7"
            }
          ]
        }
      ]
    },
    {
      "name": "Home Pages",
      "item": [
        {
          "id": "767e955d-6a33-4435-be64-9b72868b4cb6",
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
              "id": "d69acc7b-2283-4416-8165-8bebf25ee4be"
            }
          ]
        },
        {
          "id": "67c2f6cb-0bca-4da4-a254-f029e17b28be",
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
              "id": "3bfcfa6f-1a30-494c-85be-e96b6a4d5d46"
            }
          ]
        },
        {
          "id": "a846640a-b590-4711-8fe3-464977567651",
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
              "id": "269fceff-98f9-4776-82b0-750a0350fd30"
            }
          ]
        },
        {
          "id": "f542fda5-a339-4ec1-afa4-94ab274cdd2e",
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
              "id": "a7a91914-8dcb-41f6-b762-ac9c74de10a6"
            }
          ]
        },
        {
          "id": "eb50f3ed-de0b-47e4-bf04-d36ce26d7a7d",
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
              "id": "cb3d070e-feb2-482a-b5fb-4ec5c9a522d9"
            }
          ]
        },
        {
          "id": "a64fe02b-e643-4dca-890e-493c20817510",
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
              "id": "bc29cd8f-d26a-4e3d-9e41-f37b13c86f4f"
            }
          ]
        },
        {
          "id": "8a3df63b-9643-43d8-9944-dbbfc01addc4",
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
              "id": "3f2bcdb1-230d-4bf9-a365-9c27ef7d4ffb"
            }
          ]
        },
        {
          "id": "4a0a76b9-e5c3-4ac4-9dcc-a7c4fac4f279",
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
              "id": "d2f647bd-64e5-40c4-8f8e-c5e090195926"
            }
          ]
        },
        {
          "id": "51fb59a9-38bd-402d-8060-39d03a10629e",
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
              "id": "6ed9f213-ed3c-4940-9af3-ade90431e4b3"
            }
          ]
        },
        {
          "id": "6f54ffcc-3ef9-4bfc-a258-4789edbda7a7",
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
              "id": "f18a58c4-6e5d-4403-a329-a01e8742e154"
            }
          ]
        }
      ]
    },
    {
      "name": "Listings",
      "item": [
        {
          "id": "cb1a8f49-add5-4a84-b7a2-34f3c0c6ed3c",
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
              "id": "53e59c34-f7b5-410c-9e83-863d206d5f20"
            }
          ]
        },
        {
          "id": "7acad055-132b-4da4-943e-19128dcbffeb",
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
              "id": "3da8358b-0f66-4718-846e-21e6d8888b8a"
            }
          ]
        },
        {
          "id": "d958749a-a87c-46f8-adf1-5f44424d4778",
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
              "id": "7e70c88f-7db1-4ebe-88d4-a39b5c3cfd43"
            }
          ]
        },
        {
          "id": "b4451be4-21bc-4bfb-82aa-066c9c677b11",
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
              "id": "3c810c04-feb5-42f1-bb45-f0fdc1dd310f"
            }
          ]
        },
        {
          "id": "bdfb40d4-d396-4982-bae6-be0463d32971",
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
              "id": "856063ed-110e-4908-be8a-3f8599ce3acf"
            }
          ]
        },
        {
          "id": "7a6c1aff-e76b-4537-9cb6-68dbe6ee24d5",
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
              "id": "a4135626-bcd9-4e5a-b2af-fc3f6de99c05"
            }
          ]
        },
        {
          "id": "2fca37b9-1c03-4869-b205-d6ffc762736f",
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
              "id": "8d25e1cf-35ca-4ec6-8502-94be1c837edd"
            }
          ]
        },
        {
          "id": "9cc77307-a63a-40ae-95b1-ab540f63a405",
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
              "id": "39696eb1-d32a-4045-8c9f-8571ce7494c4"
            }
          ]
        },
        {
          "id": "f27f154c-5ed6-45f0-9a37-d4fc9399ba3b",
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
              "id": "c319a20e-fbdc-4fbb-95b2-40e02b502206"
            }
          ]
        },
        {
          "id": "50f64dd5-4530-4156-9e51-f42701d02643",
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
              "id": "2b7311fb-e974-43d1-a32f-ecda6a59cea3"
            }
          ]
        },
        {
          "id": "40552b80-38dd-4177-8811-785a472cea4e",
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
              "id": "7711e7af-2014-40eb-a4a0-691916e32821"
            }
          ]
        },
        {
          "id": "f9ed7337-f30c-494f-af1a-647aee9d8375",
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
              "id": "9a64ac11-cd21-4166-979e-c2f0f036eb18"
            }
          ]
        },
        {
          "id": "1bf16ddf-9e7d-454e-b327-c33e946050b3",
          "name": "postListings",
          "request": {
            "url": "http://openapi.etsy.com/v2/private/listings?description=%7B%7D&materials=%7B%7D&price=%7B%7D&quantity=%7B%7D&shipping_template_id=%7B%7D&shop_section_id=%7B%7D&tags=%7B%7D&title=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new L