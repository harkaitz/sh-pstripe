# PSTRIPE

## Help

pstripe

    Usage: pstripe [-vtE:] ...
    
    User management system integrated with stripe.
    
    ## Initial configuration.
    
    ... show                : Show configuration.
    ... tax-list            : List created taxes.
    ... tax-edit [i=ID] ... : Create/Edit tax.
        | t=TYPE j=ES n=NAME p=PERC d=DESC a=ACTIVE
    
    ## Create services.
    
    ... sub-list         : List defined subscriptions.
    ... sub-edit [i=ID]  : Create/Edit subscription.
        | n=NAME u=URL a=CENTS p=PERIOD{w,d,y,m} d=DESC
    
    ## User/customer management.
    
    ... userlist
    ... useradd      [i=1] e=EMAIL p=PASS l=LANG
    ... useradd-mail [i=1] e=EMAIL p=PASS l=LANG
    ... usermod ID OPTS...
        a_city=T   a_country=T     a_line1=T
        a_line2=T  a_postal_code=T a_state=T
        d=DESC     e=EMAIL         n=NAME
        p=PHONE    cif=NUM         pass=PASSWD
    ... userdel     CUSTOMER-ID
    ... send-verify CUSTOMER-ID
    ... test-verify CUSTOMER-ID : Print code instead of emailing.
    ... recv-verify EMAIL CODE
    
    ... login [i=1] e=EMAIL p=PASS a=AUTH > CUSTOMER-ID
    ... auths CUSTOMER-ID > SERVICES
    ... info  CUSTOMER-ID
    
    ## User checking out.
    
    ... ses-new s=ID ... : Create new session.
        c=CUSTOMER us=URL-SUCCESS uc=URL-CANCEL
        r=REFERENCE b=BROWSER

## Collaborating

For making bug reports, feature requests and donations visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)

