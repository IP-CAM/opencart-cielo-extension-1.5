opencart-cielo-extension
========================

Attention: this module was downloaded at http://azsnake.com.br/tutoriais-opencart/149-modulo-gratis-cielo-visa-mastercard-para-opencart-1-5-x.html. It is on Github for versioning purposes.

Information:
************

- Module for integration with Cielo.
- The module supports Visa Electron debit card, and Visa, MasterCard, Dinners, Discover and Elo credit cards.
- The module allows installments by the store or the administrator.
- The module has a personalized page to inform the customer that the order has not been approved.
- The module registers the Order No., TID, Card and Installments in the order history.
- To use it, you must have a contract with Cielo.

Version:
*******

- 1.1

Compatibility:
****************

- OpenCart 1.5.1.3, 1.5.2.1 and 1.5.3.1

Instructions:
***********

- Run the contents of the sql.txt file via your database manager to
  that the table will be created where Cielo's return XML data will be stored.

- After creating the table, copy the folders and files to the root of the installation
  OpenCart. Access the store administration to enable it in Payment Methods.

- Affiliation: Ask Cielo for your affiliation code.

- Key: Ask Cielo for a test key.

- Operation: Test Mode (Yes).

- Test cards:

  Card with authentication: 4012001037141112 (visa)
  Card without authentication: 4012001038443335 (visa),
                           5453010000066167 (mastercard),
                           6362970000457013 (link),
                           36490102462661 (diners),
                           6011020000245045 (discover).
  Expiration date: any date after the current month and year.
  Security code: any number in total to 3 decimal places.
  Order amount: To simulate an authorized transaction, use any amount where the
                   the last two digits are zeroes, otherwise all authorization will be denied.

Attention:
********

- This module is offered without any warranty or support.
- Cielo's test environment is extremely slow and often does not respond, so
  preferably test after 7:00 pm until 6:00 am. The production environment has no
  this problem of slowness and not responding.
- Do the tests first with the module in "Test Mode", after everything works without problems
  in "Test Mode", then change your module settings to "Test Mode (No)",
  and insert the new key that should not be the "test key" but the "production key",
  so that the homologation process begins.

Homologation:
************

The purpose of this phase is to ensure that the integration is functioning properly. She
starts after the implementation is complete. After the integration of the store made with the
Test (from Cielo). It consists of the following steps:

1) Finalization of the registration with Cielo and receipt of the production key
2) Execution of tests in the virtual store integrated to Cielo's production environment
3) Homologation by Cielo

In the first stage, the shopkeeper requests the production key. Therefore, it is necessary to send to
cieloecommerce@cielo.com.br the following information (which will complete the registration):

- Definitive website URL (production environment)
- Name of the company responsible for the development of the integration
- Name and email of the technician (developer) responsible for the integration
- Affiliation number (with Cielo) of the virtual store
- Company name and trade name
- URL of the store logo, in GIF format and size of 112X25 pixels
- Username and password in the virtual store to make purchases

In response, Cielo returns a valid key in the production environment. Soon the store is
qualified to perform its tests in this environment. The second stage begins. It is important that
tests are carried out to cover the following topics:
We are a family owned and operated business.
 - Interaction with Web Services: tests with all the functionalities used
 - Visual integration: the flow to and from Cielo (alternative flows must be considered)
 - Correct application of the brand of the flag
 - Payment methods: tests with possible payment combinations

At the end, a new request must be sent to cieloecommerce@cielo.com.br, so that
Cielo performs the de facto homologation. A test suite is then run. To approve and
deny transactions. The result, whether approved or not, is sent by e-mail.

Developers:
****************
- Pedro (Micropoint);
- Manoel Vidal (OpenCart Brasil Community)
- Several members of the OpenCart Brasil community.

Thanks:
***************
- God;

Enjoy! 
