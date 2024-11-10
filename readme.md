# SHA-256 Hashing Login System:

Login Page: When the user logs in with the correct credentials, a hash is generated based on the username and password. This hash is stored in sessionStorage for the current session.

Admin Page: When the admin.html page loads, it computes valid hashes and checks if the stored hash matches any of them. If there’s no match or the hash is missing, the user is redirected to the login page.

This solution keeps the authentication entirely client-side, suitable for demos or low-security applications. However, keep in mind that this approach isn’t highly secure, as it’s possible to manipulate sessionStorage and see the code, but it works well in local or demo environments.