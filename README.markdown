This plugin provides an easy way to include Sluggable Behavior from Mariano Iglesias in your application.

It includes a small fix to be compatible with the new CakePHP 1.2 find conditions syntax.

## Installation
- Clone from github : in your plugin directory type `git clone git://github.com/msadouni/cakephp-sluggable-plugin.git sluggable`
- Add as a git submodule : in your plugin directory type `git submodule add git://github.com/msadouni/cakephp-sluggable-plugin.git sluggable`
- Download an archive from github and extract it in `/plugins/sluggable`

## Usage
In a model that needs slugging, add :

    var $actsAs = array('Sluggable.Sluggable' => array(...))

Available options :

- label : (array | string, optional) set to the field name that contains the
    string from where to generate the slug, or a set of field names to
    concatenate for generating the slug. DEFAULTS TO: title
- slug : (string, optional) name of the field name that holds generated slugs.
    DEFAULTS TO: slug
- separator : (string, optional) separator character / string to use for replacing
    non alphabetic characters in generated slug. DEFAULTS TO: -
- length : (integer, optional) maximum length the generated slug can have.
    DEFAULTS TO: 100
- overwrite : (boolean, optional) set to true if slugs should be re-generated when
    updating an existing record. DEFAULTS TO: false

Source : [Cake Syrup](http://cake-syrup.sourceforge.net/ingredients/sluggable-behavior/)