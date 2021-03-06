Class **Phalcon\\Http\\Response\\Headers**
==========================================

*implements* :doc:`Phalcon\\Http\\Response\\HeadersInterface <Phalcon_Http_Response_HeadersInterface>`

.. role:: raw-html(raw)
   :format: html

:raw-html:`<a href="https://github.com/dreamsxin/cphalcon7/blob/master/ext/http/response/headers.c" class="btn btn-default btn-sm">Source on GitHub</a>`

This class is a bag to manage the response headers


Methods
-------

public  **set** (*string* $name, *string* $value)

Sets a header to be sent at the end of the request



public *string*  **get** (*string* $name)

Gets a header value from the internal bag



public  **setRaw** (*string* $header)

Sets a raw header to be sent at the end of the request



public  **remove** (*unknown* $header_index)

Removes a header to be sent at the end of the request



public *boolean*  **send** ()

Sends the headers to the client



public  **reset** ()

Reset set headers



public *array*  **toArray** ()

Returns the current headers as an array



public static :doc:`Phalcon\\Http\\Response\\Headers <Phalcon_Http_Response_Headers>`  **__set_state** (*array* $data)

Restore a Phalcon\\Http\\Response\\Headers object



