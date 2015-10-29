# showterm
The alternative to the rubygem. This is a bash client script used to
record a terminal and then to upload the recording files to _showterm.io_.

This fork has more robust error handling and uses the XDG
formalities from Freedesk.org to locate places under user's $HOME 
to save screen record files.

## 

The file _showterm_ in the top level on branch "altern-bash-client" is not
in the upstream repo (owned by Conrad Irwin).
I rewrote the logic because I consistently got non-zero return on upload
even if the upload succeeded, shown as success by cURL printing the reply
( the "playback URL") sent by the server.  The error return "6" by cURL is
spurious (not a real error) ...other releases of cURL might not return "6".
      
I've changed display of lines showing progress so that "new playback URL"
printed by cURL appears on separate line for easier copying ...you'll see.
It is a bit difficult to describe the normal output of this tool.

Clone this script from the branch *altern-bash-client*.
