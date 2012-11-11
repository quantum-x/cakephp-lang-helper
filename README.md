CakePHP Language and Country Helper cakephp 2.x
===================================

License
-------

Some snippets taken from Tane Piper See http://digitalspaghetti.me.uk
Author: Brendon Crawford
See: http://github.com/brendoncrawford/cakephp-lang-helper

Licensed under The MIT License
Redistributions of files must retain the above copyright notice.

Summary
-------

Outputs a country select list and/or a language select list. Automatically
detects language and country codes from browser headers.

Usage
-----

Helper Class:

    <?php  echo $this->lang->countrySelect('Foo.country'); ?>

Helper Class:

    <?php  echo $this->lang->languageSelect('Foo.language'); ?>

You can override defaults such as:

Helper Class:

    <?php 
    echo $this->lang->countrySelect('Foo.country', array(
        'label' => __('Choose a Country', true),
        'default' => 'ru',
        'class' => 'some-class'
    ));
    ?>

Helper Class:

    <?php 
        echo $this->lang->languageSelect('Foo.language', array(
            'label' => __('Choose a Language', true),
            'default' => 'sp',
            'class' => 'some-class'
       ));
    ?>

Note that the 'default' option is only used if the form was not previously
submitted, and country/language information could not be extracted from
the HTTP request.
