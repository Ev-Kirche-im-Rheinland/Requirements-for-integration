# Requirements-for-integration

Version: 1.0.1

Requirements for integration of a web application into the EKIR portal

# 1. About the web application
- The web application must be executable in the browser (reference Google Chrome) without additional browser plugins (native).
- Access to the web application must be mandatory from the WWW, without network restrictions (VPN).
- The integration into the portal ideally takes place in the iFrame

# 2. Operation and Compliance
- The operation of the web application (hereinafter business application) must comply our regulatory requirements (DSG-EKD, ITSVO, ISO27001 etc).
- Provision in an ISO certified data center in EUROPE is a prerequisite.
- The technical guidelines (https://github.com/Ev-Kirche-im-Rheinland) of the EKIR must be fulfilled 

# 3. Single-Sign-On
- User administration (roles, rights) always takes place in business application; the EKIR portal (as IDP) provides all users as identities.
- An SSO (single sign-on) and an SLO (single sign-off) must be established. OpenID Connect (OIDC) or SAML (until the end of 2025) is used for this.
- Keycloak should be used on the business application side. EKIR provides an import template for Keycloak.
- The technical specification for the use of OIDC / SAML must be observed.
- Additional user information can be exchanged via the REST API (option).

# 4. Organization
- A person responsible for the business application (contact person, administration) must be permanently available.
- Persons responsible for the business application participate in the quality circle of the EKiR.

# 5. Costs
- The costs for integrating the portal must be determined individually for each project depending on the respective requirements 
and are to be borne by the client of the business application.
