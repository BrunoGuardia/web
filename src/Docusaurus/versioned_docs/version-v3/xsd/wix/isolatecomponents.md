---
title: IsolateComponents Element
layout: documentation_xsd_main
---
<dl>
  <dt>Description</dt>
  <dd>Installs a copy of a component (commonly a shared DLL) into a private location for use by a specific application (typically an .exe).  This isolates the application from other copies of the component that may be installed to a shared location on the computer.  The action refers to each record of the IsolatedComponent table and associates the files of the component listed in the Component_Shared field with the component listed in the Component_Application field.  The installer installs the files of Component_Shared into the same directory as Component_Application.  The installer generates a file in this directory, zero bytes in length, having the short filename name of the key file for Component_Application (typically this is the same file name as the .exe) appended with .local.  The IsolatedComponent action does not affect the installation of Component_Application.  Uninstalling Component_Application also removes the Component_Shared files and the .local file from the directory.  The IsolateComponents action can be used only in the InstallUISequence table and the InstallExecuteSequence table.  This action must come after the CostInitialize action and before the CostFinalize action.  The condition for this action may be specified in the element's inner text.</dd>
  <dt>Windows Installer references</dt>
  <dd>
    <a href="http://msdn.microsoft.com/library/aa369561.aspx" target="_blank">IsolateComponents Action</a>
  </dd>
  <dt>Parents</dt>
  <dd>
    <a href="../wix/installexecutesequence">InstallExecuteSequence</a>, <a href="../wix/installuisequence">InstallUISequence</a></dd>
  <dt>Inner Text (xs:string)</dt>
  <dd>This element may have inner text.</dd>
  <dt>Children</dt>
  <dd>None</dd>
  <dt>Attributes</dt>
  <dd>
    <table cellspacing="0" cellpadding="0" class="schema">
      <tr>
        <th width="15%">Name</th>
        <th width="15%">Type</th>
        <th width="65%">Description</th>
        <th width="15%">Required</th>
      </tr>
      <tr>
        <td>Sequence</td>
        <td>Integer</td>
        <td>A value used to indicate the position of this action in a sequence.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Suppress</td>
        <td><a href="../wix/simple_type_yesnotype">YesNoType</a></td>
        <td>If yes, this action will not occur.</td>
        <td>&nbsp;</td>
      </tr>
    </table>
  </dd>
  <dt>See Also</dt>
  <dd>
    <a href="../wix">Wix Schema</a>, <a href="../wix/isolatecomponent">IsolateComponent</a></dd>
</dl>
