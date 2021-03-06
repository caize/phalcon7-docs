Abstract class **Phalcon\\Session\\Adapter**
============================================

*implements* :doc:`Phalcon\\Session\\AdapterInterface <Phalcon_Session_AdapterInterface>`, Countable, IteratorAggregate, Traversable, ArrayAccess

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/session/adapter.c" class="btn btn-default btn-sm">Source on GitHub</a>`

Base class for Phalcon\\Session adapters


Methods
-------

public  **__construct** ([*array* $options], [*int* $expire], [*string* $path], [*boolean* $secure], [*string* $domain], [*boolean* $httpOnly])

Phalcon\\Session\\Adapter constructor



public  **__destruct** ()

...


public *boolean*  **start** ()

Starts the session (if headers are already sent the session will not be started)



public  **setOptions** (*array* $options)

Sets session's options 

.. code-block:: php

    <?php

    $session->setOptions(array(
    	'uniqueId' => 'my-private-app'
    ));




public *array*  **getOptions** ()

Get internal options



public *mixed*  **get** (*string* $index, [*mixed* $defaultValue])

Gets a session variable from an application context



public  **set** (*string* $index, *string* $value)

Sets a session variable in an application context 

.. code-block:: php

    <?php

    $session->set('auth', 'yes');




public  **sets** (*array* $data)

Sets a session variables in an application context 

.. code-block:: php

    <?php

    $session->sets(array('auth', 'yes'));




public *boolean*  **has** (*string* $index)

Check whether a session variable is set in an application context 

.. code-block:: php

    <?php

    var_dump($session->has('auth'));




public  **remove** (*string* $index)

Removes a session variable from an application context 

.. code-block:: php

    <?php

    $session->remove('auth');




public *string*  **getId** ()

Returns active session id 

.. code-block:: php

    <?php

    echo $session->getId();




public *boolean*  **isStarted** ()

Check whether the session has been started 

.. code-block:: php

    <?php

    var_dump($session->isStarted());




public *boolean*  **regenerate** ([*unknown* $delete_old_session])

Update the current session id with a newly generated one  

.. code-block:: php

    <?php

    var_dump($session->regenerate());




public *boolean*  **destroy** ([*unknown* $regenerate])

Destroys the active session 

.. code-block:: php

    <?php

    var_dump($session->destroy());




public  **__get** (*unknown* $property)

...


public  **__set** (*unknown* $property, *unknown* $value)

...


public  **__isset** (*unknown* $property)

...


public  **__unset** (*unknown* $property)

...


public  **offsetGet** (*unknown* $property)

...


public  **offsetSet** (*unknown* $property, *unknown* $value)

...


public  **offsetExists** (*unknown* $property)

...


public  **offsetUnset** (*unknown* $property)

...


public  **count** ()

...


public  **getIterator** ()

...


public  **setId** (*unknown* $sid)

Set the current session id 

.. code-block:: php

    <?php

    $session->setId($id);




