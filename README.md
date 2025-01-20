# Incorrectly Nested Paragraph Tag in Dynamically Added innerHTML

This repository demonstrates a subtle HTML bug involving incorrectly nested paragraph tags when using `innerHTML` to dynamically add content. The bug can lead to unexpected rendering results and potentially fail HTML validation.

## Bug Description
The bug arises from inserting a `<p>` tag inside a dynamically created `innerHTML` which itself was inside a `<div>` tag without proper structure.  Modern browsers might render this, but this approach is not semantically correct and can cause inconsistencies across different browsers or validation errors. 

## Solution
The solution involves ensuring that the content added via `innerHTML` maintains the correct semantic structure. This example uses a safe method of concatenating strings which will avoid the issue. 