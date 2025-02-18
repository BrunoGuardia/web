---
title: DirectorySearch Element (Util Extension)
layout: documentation_xsd_extension
---
<dl>
  <dt>Description</dt>
  <dd>Describes a directory search.</dd>
  <dt>Windows Installer references</dt>
  <dd>None</dd>
  <dt>Parents</dt>
  <dd>
    <a href="../wix/bundle">Bundle</a>, <a href="../wix/fragment">Fragment</a></dd>
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
        <td>After</td>
        <td>String</td>
        <td>Id of the search that this one should come after.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Condition</td>
        <td>String</td>
        <td>Condition for evaluating the search. If this evaluates to false, the search is not executed at all.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Id</td>
        <td>String</td>
        <td>Id of the search for ordering and dependency.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Path</td>
        <td>String</td>
        <td>Directory path to search for.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Result</td>
        <td>NMTOKEN</td>
        <td>             Rather than saving the matching directory path into the variable, a DirectorySearch can save an             attribute of the matching directory instead.             Pattern: 'exists'.</td>
        <td>&nbsp;</td>
      </tr>
      <tr>
        <td>Variable</td>
        <td>String</td>
        <td>Name of the variable in which to place the result of the search.</td>
        <td>Yes</td>
      </tr>
    </table>
  </dd>
  <dt>See Also</dt>
  <dd>
    <a href="../util">Util Schema</a>
  </dd>
</dl>
