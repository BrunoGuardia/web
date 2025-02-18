---
title: Family Element
layout: documentation_xsd_main
---
<dl>
  <dt>Description</dt>
  <dd>Group of one or more upgraded images of a product.</dd>
  <dt>Windows Installer references</dt>
  <dd>None</dd>
  <dt>Parents</dt>
  <dd>
    <a href="../wix/patchcreation">PatchCreation</a>
  </dd>
  <dt>Inner Text</dt>
  <dd>None</dd>
  <dt>Children</dt>
  <dd>Sequence (min: 1, max: 1)<ol><li><a href="../wix/upgradeimage">UpgradeImage</a> (min: 1, max: unbounded)</li><li>Choice of elements (min: 0, max: unbounded)<ul><li><a href="../wix/externalfile">ExternalFile</a> (min: 0, max: unbounded)</li><li><a href="../wix/protectfile">ProtectFile</a> (min: 0, max: unbounded)</li></ul></li></ol></dd>
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
        <td>DiskId</td>
        <td><a href="../wix/simple_type_diskidtype">DiskIdType</a></td>
        <td>Entered into the DiskId field of the new Media table record.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>DiskPrompt</td>
        <td>String</td>
        <td>Value to display in the "[1]" of the DiskPrompt Property.  Using this attribute will require you to define a DiskPrompt Property.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>MediaSrcProp</td>
        <td>String</td>
        <td>Entered into the Source field of the new Media table entry of the upgraded image.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Name</td>
        <td>String</td>
        <td>Identifier for the family.</td>
        <td>Yes</td>
      </tr>
      <tr>
        <td>SequenceStart</td>
        <td>Int</td>
        <td>Sequence number for the starting file.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>VolumeLabel</td>
        <td>String</td>
        <td>Entered into the VolumeLabel field of the new Media table record.</td>
        <td>&nbsp;</td>
      </tr>
    </table>
  </dd>
  <dt>See Also</dt>
  <dd>
    <a href="../wix">Wix Schema</a>
  </dd>
</dl>
