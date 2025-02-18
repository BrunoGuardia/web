---
title: String Element (Wixloc Extension)
layout: documentation_xsd_extension
---
<dl>
  <dt>Description</dt>
  <dd>None</dd>
  <dt>Windows Installer references</dt>
  <dd>None</dd>
  <dt>Parents</dt>
  <dd>
    <a href="../wixloc/wixlocalization" class="extension">WixLocalization</a>
  </dd>
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
        <td>Id</td>
        <td>String</td>
        <td>Identity of the resource.</td>
        <td>Yes</td>
      </tr>
      <tr>
        <td>Localizable</td>
        <td><a href="../wixloc/simple_type_localizationyesnotype">LocalizationYesNoType</a></td>
        <td>Indicates whether the string is localizable text or a non-localizable string that must be unique per locale. No WiX tools are affected by the value of this attribute; it used as documentation for localizers to ignore things like GUIDs or identifiers that look like text.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Overridable</td>
        <td><a href="../wixloc/simple_type_localizationyesnotype">LocalizationYesNoType</a></td>
        <td>Determines if the localized string may be overridden.</td>
        <td>&nbsp;</td>
      </tr>
    </table>
  </dd>
  <dt>How Tos and Examples</dt>
  <dd>
    <ul>
      <li>
        <a href="../../howtos/ui_and_localization/build_a_localized_version">How To: Build a localized version of your installer</a>
      </li>
      <li>
        <a href="../../howtos/ui_and_localization/make_installer_localizable">How To: Make your installer localizable</a>
      </li>
    </ul>
  </dd>
  <dt>See Also</dt>
  <dd>
    <a href="../wixloc">Wixloc Schema</a>
  </dd>
</dl>
