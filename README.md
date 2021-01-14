# csci1301-site
Website for CSCI 1301 at Brown University, which can be found here: https://cs.brown.edu/courses/cs1301/.

# instructions
A useful script is the `update_to_775_permissions script`. This will simply update permissions to be read-write-execute for all cs1301tas and the user, and then read-execute for all other users. One thing to note is that sometimes there is a permission mismatch with folders, which causes the site to crash (because the department filesystem can't access a folder). To solve this on a department machine, right click on the folder, go to the permissions tab, and there should be a prompt that tells you how to fix the permissions.

In order to update the CSCI 1301 homepage, navigate to `/web/cs/web/courses/csci1301/` on a department machine. From there, simply `git pull` this repo.
If you're developing locally, `git clone` first, make any changes, add and commit everything, and push. Then, pull on a department machine in the csci1301 directory. If nothing loads on the site anymore, it is likely that permissions changed when you pulled. To fix this, run the script above, or manually update the "Others" permissions to "Read Only," which allows the department system to read any relevant files. Never allow "Others" to have write permissions, as that means anyone at Brown can change the site's code.

# credits
The vast majority of the structure of this site was copied from the CSCI 1300 site, https://cs.brown.edu/courses/csci1300/, which is a class about UI/UX. Surely that should be a good base for a site, right?


