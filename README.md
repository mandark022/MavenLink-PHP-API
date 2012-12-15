MavenLink-PHP-API
=================

Example:

require('api/mavenlink.php');
$mapi = MavenLink(userid,token);


//Get all workspaces
$data - $mapi->getWorkspaces();
var_dump(json_decode($data));


//Get A Specific Workspace Information
$data - $mapi->getWorkspaces(<workspaceid>);
var_dump(json_decode($data));


//Create A Workspace
$data - $mapi->createWorkspace(array('title'=>'MyTitle','creator_role'=>'maven'));
var_dump(json_decode($data));


//Update Workspace
$data - $mapi->updateWorkspace(array('title'=>'MyTitle is Updated','description'=>'Update'));
var_dump(json_decode($data));
