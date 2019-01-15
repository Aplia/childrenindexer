# Children Indexer
eZPublish extension which allows you to index subitems as an attribute of the parent node. It also works with eZFind.

## Description
Children indexer allows to return parent nodes when searching for a term occurring in their (helper) child nodes. For example, by using this extension it is possible to return an article or a forum thread when searching for a term occurring in a related article comment or a forum post.

To use the extension, add a "Reindex parent node" event to the workflow triggered after content is published. You also need to add an attribute of the "Children indexer" datatype to classes used as master nodes. If your site already has some content, you must re-index your site by running bin/php/updatesearchindex.php.

## Installation
Install with Composer:
	```
	composer require aplia/childrenindexer
	```