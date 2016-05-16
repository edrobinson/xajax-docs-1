## Response->domRemoveChildren()

Signature: public function domRemoveChildren($parent, $skip = null, $remove = null)

Parameters:

* $parent
* $skip = null
* $remove = null

Description:
The domRemoveChildren method is used to 

Example:
<code><pre>
function domRemoveChildrenExample()
{
    $oResponse = new Response()
    $oResponse->domRemoveChildren()
    return $oResponse
}
</pre></code>