## Onboarding API Vocabulary

### Data Elements

##### Onboarding Data

 * onboardingId (r)
 * [CompanyData]
 * [AccountData]
 * [ActivityData]
 * status (r)(e)
 * dateCreated
 * dateUpdated

 Valid _status_ values are:

  * working
  * cancelled
  * completed

#### CompanyData

* companyId (r)
* companyName (r)
* streetAddress
* city
* stateProvince
* postalCode
* country
* telephone
* email
* status (r)
* dateCreated
* dateUpdated 

Valid _status_ values are:

 * pending
 * active
 * suspended
 * closed

#### AccountData

* accountId
* division (r)(e))
* companyId (r)
* spendingLimit
* discountPercentage
* status (r)(e)
* dateCreated
* dateUpdated

The value for _companyId_ MUST be unique

Valid _division_ values are:

 - DryGoods
 - Hardware
 - Software
 - Grocery
 - Pharmacy
 - Military

Valid _status_ values are:
 - suspended
 - pending
 - active
 - closed

#### ActivityData

* activityId
* activityType (r)(e)
* companyId (r)
* accountId
* dataScheduled
* notes
* status (r)(e)
* dateCreated
* dateUpdated

Valid _activityType_ values are:
- email
- inperson
- phone
- letter

Valid _status_ values are:
 - suspended
 - pending
 - active
 - closed




