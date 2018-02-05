# Remote-Access-Policy-Enumeration
Find systems where pass the hash will work for non rid 500 accounts . Will search for enable LUA and LocalAccountTokenFilterPolicy

# Blog Post

https://labs.mwrinfosecurity.com/blog/enumerating-remote-access-policies-through-gpo/

# Usage

Check GPO for settings which deal with remote access policies relevant to lateral movement
(e.g., "EnableLUA" and "LocalAccountTokenFilterPolicy").  The OUs to which these GPOs are applied 
are then identified, and then the computer objects from each are retrieved.  Note that this only 
retrieves computer objects who have had the relevent registry keys set through group policy.

 Find-ComputersWithRemoteAccessPolicies
 or
 Find-ComputersWithRemoteAccessPolicies -Domain dev.testlab.local
 
 
