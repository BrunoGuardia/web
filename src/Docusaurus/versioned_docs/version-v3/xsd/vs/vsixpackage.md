---
title: VsixPackage Element (Vs Extension)
layout: documentation_xsd_extension
---
<dl>
  <dt>Description</dt>
  <dd>                 This element provides the metdata required to install/uninstall a file as                 a VSIX Package. The VSIX package file will be installed as part of the MSI                 then passed to the VSIX installer to install the VSIX package. To avoid the                 duplication, simply use the MSI to install the VSIX package itself.             </dd>
  <dt>Windows Installer references</dt>
  <dd>None</dd>
  <dt>Parents</dt>
  <dd>
    <a href="../wix/component">Component</a>, <a href="../wix/file">File</a></dd>
  <dt>Inner Text</dt>
  <dd>None</dd>
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
        <td>File</td>
        <td>String</td>
        <td>                     Reference to file identifer. This attribute is required when the element is not a                     child of a File element and is invalid when the element is a child of the File element.                     </td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>PackageId</td>
        <td>String</td>
        <td>                     Identity of the VSIX package per its internal manifest. If this value is not correct                     the VSIX package will not correctly uninstall.                     </td>
        <td>Yes</td>
      </tr>
      <tr>
        <td>Permanent</td>
        <td><a href="../vs/simple_type_yesnotype">YesNoType</a></td>
        <td>                     Indicates whether the VSIX package is uninstalled when the parent Component is uninstalled.                     The default is 'no'.                     </td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Target</td>
        <td>String</td>
        <td>                     Specifies the SKU of Visual Studio in which to register the extension. If no target                     is specified the extension is registered with all installed SKUs. If the Target                     attribute is specified the TargetVersion attribute must also be specified. The                      following is a list of known Visual Studio targets: integratedShell, professional,                     premium, ultimate, vbExpress, vcExpress, vcsExpress, vwdExpress                     </td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>TargetVersion</td>
        <td><a href="../vs/simple_type_versiontype">VersionType</a></td>
        <td>                     Specifies the version of Visual Studio in which to register the extension. This attribute                     is required if the Target attribute is specified.                     </td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Vital</td>
        <td><a href="../vs/simple_type_yesnotype">YesNoType</a></td>
        <td>                     Indicates whether failure to install the VSIX package causes the installation to rollback.                     The default is 'yes'.                     </td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>VsixInstallerPathProperty</td>
        <td>String</td>
        <td>                     Optional reference to a Property element that contains the path to the VsixInstaller.exe.                     By default, the latest VsixInstaller.exe on the machine will be used to install the VSIX                     package. It is highly recommended that this attribute is *not* used.                     </td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td colspan="4">
          <span class="extension">Any Attribute (namespace='##other' processContents='lax')                      Extensibility point in the WiX XML Schema.  Schema extensions can register additional                     attributes at this point in the schema.                 </span>
        </td>
      </tr>
    </table>
  </dd>
  <dt>See Also</dt>
  <dd>
    <a href="../vs">Vs Schema</a>
  </dd>
</dl>
