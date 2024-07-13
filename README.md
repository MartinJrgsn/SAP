# Standardized Authentication Protocol (SAP)

When accessing services on the internet today we are often asked to register.
Each website you register with increases your risk of losing the information
you provide to these services, both during and after registering.

What I am suggesting is one standard authentication protocol that serves both
the service implementing the protocol by reducing another component to
maintain, the authority for providing security to their citizens, and the user
for the simplified, and increased Security and Privacy by giving the user
control over the data they want to share with a specific website.

The service only needs to implement authentication once for one unified system.
The service only needs to concern themselves with their content and products,
while allowing governments to handle authorization for different categories,
such as age restriction and limitations for different types of content.

## User Story

The user accesses a service and recognizes a need to register. They click the
register button and meet an implementation of this new standardized protocol,
the Standardized Authentication Mechanism. The user is presented with the SAM
login screen where they supply their password, and are consequently prompted
for their two-factor authentication TOTP. After accepting the sign-in attempt,
they are met with the SAM Registration (SAMR) screen. This screen is the result
of a handshake between the service and the user's governing authority. The
service has requested to create a new user, and they wish to use the user's
private information (name, e-mail address, phone number, geolocation, home
address, birthdate). Based on the category of the service, which is defined by 
the service, the user, and the authority, the authority agrees that the service
can get specific types of information. The user can then agree with the
authority fully, or they can toggle different fields of information. It is now
up to the service to handle potential missing information, by either creating a
pseudonym for the user in the event of a missing name or by conceptualizing
different methods of contacting the user if the user decides not to share their
contact information.

The goal is an increased level of control over their privacy. It also serves to
inform the user of the specific types of data that is shared with a service,
with the opportunity to outright deny the service any information regarding the
user. This opens for a need for an authority that can take on the
responsibility to ensure privacy and security on the internet for their
citizens.

## The Simplified Logic

There are three parts: The service, the authority, and the user. As an example,
the service requests the authority to share the following data about the user:

- First Name(s)
- Surname
- Date of Birth
- Gender Identity
- Sexual Orientation
- Phone Number
- E-mail Address
- Home Address
- Work Address
- Education Records

If the service is of the category, Cinema Streaming, the authority may approve
that it is reasonable to share the following information:

- First Name(s)
- Surname
- Date of Birth
- Gender Identity
- Sexual Orientation
- Phone Number
- E-mail Address
- Home Address

The user is then met with the options listed above, and may select which fields
of information they are comfortable with sharing. They might select to share
the following:

- First Name(s)
- Date of Birth
- Gender Identity
- E-mail Address

The service receives the following information, and it will be up to the
service to decide how to efficiently utilize this data to serve the user.

### Note: Ephemeral data sharing

The server is never allowed to permanently store personal data on their
servers, as that could be in breach of future privacy laws. Instead, the SAM is
used to sign in, and for each request or session that requires some form of
authorization, IE. viewing age restricted movies. The service requests
authorization from the authority to present this type of data to this user. 
This would be based on the user's prior approval of using their date of birth
for this type of authorization.

