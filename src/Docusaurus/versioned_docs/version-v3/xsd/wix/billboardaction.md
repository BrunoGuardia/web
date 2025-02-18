---
title: BillboardAction Element
layout: documentation_xsd_main
---
<dl>
  <dt>Description</dt>
  <dd>                 Billboard action during which child Billboards are displayed             </dd>
  <dt>Windows Installer references</dt>
  <dd>
    <a href="http://msdn.microsoft.com/library/aa367823.aspx" target="_blank">Billboard Table</a>, <a href="http://msdn.microsoft.com/library/aa367818.aspx" target="_blank">BBControl Table</a></dd>
  <dt>Parents</dt>
  <dd>
    <a href="../wix/ui">UI</a>
  </dd>
  <dt>Inner Text</dt>
  <dd>None</dd>
  <dt>Children</dt>
  <dd>Sequence (min: 1, max: 1)<ol><li><a href="../wix/billboard">Billboard</a> (min: 1, max: unbounded): Order of Billboard elements determines order of display</li></ol></dd>
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
        <td>Action name that determines when the Billboard should be shown.</td>
        <td>Yes</td>
      </tr>
    </table>
  </dd>
  <dt>See Also</dt>
  <dd>
    <a href="../wix">Wix Schema</a>
  </dd>
</dl>
