---
title: DiskIdType (Simple Type)
layout: documentation_xsd_simpletype
---
<dl>
  <dt>Description</dt>
  <dd>Values of this type must be an integer or the value of one or more preprocessor variables with the format $(var.Variable) where "Variable" is the name of the preprocessor variable.</dd>
  <dt>Pattern Type</dt>
  <dd>Must match the regular expression: '((\d+)|(\$\(\w+\.(\w|[.])+\)))+'.</dd>
  <dt>See Also</dt>
  <dd>
    <a href="../wix">Wix Schema</a>
  </dd>
</dl>
