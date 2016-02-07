.. _class_MainLoop:

MainLoop
========

**Inherits:** :ref:`Object<class_object>`

**Inherited By:** :ref:`SceneTree<class_scenetree>`

**Category:** Core

Brief Description
-----------------

Main loop is the abstract main loop base class.

Member Functions
----------------

+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`_finalize<class_MainLoop__finalize>`  **(** **)** virtual                                               |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`_idle<class_MainLoop__idle>`  **(** :ref:`float<class_float>` delta  **)** virtual                      |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`_initialize<class_MainLoop__initialize>`  **(** **)** virtual                                           |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`_input_event<class_MainLoop__input_event>`  **(** :ref:`InputEvent<class_inputevent>` ev  **)** virtual |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`_input_text<class_MainLoop__input_text>`  **(** :ref:`String<class_string>` text  **)** virtual         |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`_iteration<class_MainLoop__iteration>`  **(** :ref:`float<class_float>` delta  **)** virtual            |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`input_event<class_MainLoop_input_event>`  **(** :ref:`InputEvent<class_inputevent>` ev  **)**           |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`input_text<class_MainLoop_input_text>`  **(** :ref:`String<class_string>` text  **)**                   |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`init<class_MainLoop_init>`  **(** **)**                                                                 |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`  | :ref:`iteration<class_MainLoop_iteration>`  **(** :ref:`float<class_float>` delta  **)**                      |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| :ref:`bool<class_bool>`  | :ref:`idle<class_MainLoop_idle>`  **(** :ref:`float<class_float>` delta  **)**                                |
+--------------------------+---------------------------------------------------------------------------------------------------------------+
| void                     | :ref:`finish<class_MainLoop_finish>`  **(** **)**                                                             |
+--------------------------+---------------------------------------------------------------------------------------------------------------+

Numeric Constants
-----------------

- **NOTIFICATION_WM_MOUSE_ENTER** = **3**
- **NOTIFICATION_WM_MOUSE_EXIT** = **4**
- **NOTIFICATION_WM_FOCUS_IN** = **5**
- **NOTIFICATION_WM_FOCUS_OUT** = **6**
- **NOTIFICATION_WM_QUIT_REQUEST** = **7**
- **NOTIFICATION_WM_UNFOCUS_REQUEST** = **8**
- **NOTIFICATION_OS_MEMORY_WARNING** = **9**

Description
-----------

Main loop is the abstract main loop base class. All other main loop classes are derived from it. Upon application start, a :ref:`MainLoop<class_mainloop>` has to be provided to OS, else the application will exit. This happens automatically (and a :ref:`SceneMainLoop<class_scenemainloop>` is created), unless a main :ref:`Script<class_script>` is supplied, which may or not create and return a :ref:`MainLoop<class_mainloop>`.

Member Function Description
---------------------------

.. _class_MainLoop__finalize:

- void  **_finalize**  **(** **)** virtual

.. _class_MainLoop__idle:

- void  **_idle**  **(** :ref:`float<class_float>` delta  **)** virtual

.. _class_MainLoop__initialize:

- void  **_initialize**  **(** **)** virtual

.. _class_MainLoop__input_event:

- void  **_input_event**  **(** :ref:`InputEvent<class_inputevent>` ev  **)** virtual

.. _class_MainLoop__input_text:

- void  **_input_text**  **(** :ref:`String<class_string>` text  **)** virtual

.. _class_MainLoop__iteration:

- void  **_iteration**  **(** :ref:`float<class_float>` delta  **)** virtual

.. _class_MainLoop_input_event:

- void  **input_event**  **(** :ref:`InputEvent<class_inputevent>` ev  **)**

.. _class_MainLoop_input_text:

- void  **input_text**  **(** :ref:`String<class_string>` text  **)**

.. _class_MainLoop_init:

- void  **init**  **(** **)**

.. _class_MainLoop_iteration:

- :ref:`bool<class_bool>`  **iteration**  **(** :ref:`float<class_float>` delta  **)**

.. _class_MainLoop_idle:

- :ref:`bool<class_bool>`  **idle**  **(** :ref:`float<class_float>` delta  **)**

.. _class_MainLoop_finish:

- void  **finish**  **(** **)**

