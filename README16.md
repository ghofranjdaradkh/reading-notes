 ## What does it mean to authenticate a user?

Authentication is the process of verifying the identity of a user or entity.

The AuthenticationManager interface in Spring Security provides a method called authenticate(), which is responsible for authenticating a user.


 ## What does it mean to authorize a user?

Once authentication is successful, the next step is authorization, which determines what actions or resources a user is allowed to access.

Spring Security uses an AccessDecisionManager to handle authorization decisions. It delegates to a chain of AccessDecisionVoter instances.

An AccessDecisionVoter considers an Authentication object and a secure object (representing a resource to be accessed) decorated with ConfigAttributes.

ConfigAttributes represent rules or permissions required to access a resource.

The AccessDecisionManager typically uses an affirmative-based approach, granting access if any voter approves it.

Users often define ConfigAttributes using Spring Expression Language (SpEL) expressions, which allows for flexible and dynamic authorization rules.




## What are the three possible outcomes of the AuthenticationManager’s authenticate() method?

Return an Authentication object (usually with authenticated=true) if the input represents a valid principal (successful authentication).
Throw an AuthenticationException if the input represents an invalid principal (failed authentication).
Return null if it cannot decide.

=======================================================
## Spring Auth Cheat Sheet

Step 1: set up a user model and repo

Step 2: create a controller for that model

Step 3: UserDetailsServiceImpl implements UserDetailsService

Step 4: ApplicationUser implements UserDetails

Step 5: WebSecurityConfig extends WebSecurityConfigurerAdapter

Step 6: registration page

Step 7: login page