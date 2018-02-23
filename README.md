# LCUAdmin
Laravel Company and User Admin

ACL - Action/Control/Layer
Convention over configuration
Facades (factory)
"PHP magical 'get' and 'set'" - 

kint - "dump utility"

"Smart defaults" - Nate Denlinger

## Dependancies
1. Laravel (> laravel make:auth)

## Application Requirements

As a basis for a new SASS application I would love to have a modular installed package that gives me the basic functionality needed in 90% of Sass applications.

This functionality includes:

* Normal user registration
* Admin can create payment plans, including a free plan
* Any user can create a Organization, they become the manager of the Organization, free plan auto selected
* Organization managers can invite other users to the Organization and specify their role (manager|employee)
* Invites are done via email address, if user exists sends them an email with a link to connect, if not the user registers then is connected
* Managers of an organization can enter in payment info for their organization, creates a stripe customer
* Managers of and organization can select a plan for the organization, charges correct amount
* Cron job to charge organization each month (stripe payment)
* Since users can belong to many organizations need a way to switch between organizations they are currently viewing/managing

### Project Work Tasks

1. Build data storage
    1. [organizations]
    2. [users] (using > laravel make:auth)
        - Add [admin]
        - type 'boolean'
    4. [organization_user]
    5. [roles]


### Phases
1. Document Phase
    1. Document high level project detail
    2. Write out description details for each database tables and clases
    3. Go through each table and add all field names
    4. If this is an API document endpoint contract
2. Code Phase
    1. 
