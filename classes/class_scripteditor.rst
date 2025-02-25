:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the ScriptEditor.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_ScriptEditor:

ScriptEditor
============

**Inherits:** :ref:`PanelContainer<class_PanelContainer>` **<** :ref:`Container<class_Container>` **<** :ref:`Control<class_Control>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

Godot editor's script editor.

Description
-----------

**Note:** This class shouldn't be instantiated directly. Instead, access the singleton using :ref:`EditorInterface.get_script_editor<class_EditorInterface_method_get_script_editor>`.

Methods
-------

+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`ScriptEditorBase<class_ScriptEditorBase>` | :ref:`get_current_editor<class_ScriptEditor_method_get_current_editor>` **(** **)** |const|                                                                                                |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Script<class_Script>`                     | :ref:`get_current_script<class_ScriptEditor_method_get_current_script>` **(** **)**                                                                                                        |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`                       | :ref:`get_open_script_editors<class_ScriptEditor_method_get_open_script_editors>` **(** **)** |const|                                                                                      |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Array<class_Array>`                       | :ref:`get_open_scripts<class_ScriptEditor_method_get_open_scripts>` **(** **)** |const|                                                                                                    |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`goto_line<class_ScriptEditor_method_goto_line>` **(** :ref:`int<class_int>` line_number **)**                                                                                        |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`open_script_create_dialog<class_ScriptEditor_method_open_script_create_dialog>` **(** :ref:`String<class_String>` base_name, :ref:`String<class_String>` base_path **)**             |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`register_syntax_highlighter<class_ScriptEditor_method_register_syntax_highlighter>` **(** :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` syntax_highlighter **)**     |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                            | :ref:`unregister_syntax_highlighter<class_ScriptEditor_method_unregister_syntax_highlighter>` **(** :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` syntax_highlighter **)** |
+-------------------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Signals
-------

.. _class_ScriptEditor_signal_editor_script_changed:

- **editor_script_changed** **(** :ref:`Script<class_Script>` script **)**

Emitted when user changed active script. Argument is a freshly activated :ref:`Script<class_Script>`.

----

.. _class_ScriptEditor_signal_script_close:

- **script_close** **(** :ref:`Script<class_Script>` script **)**

Emitted when editor is about to close the active script. Argument is a :ref:`Script<class_Script>` that is going to be closed.

Method Descriptions
-------------------

.. _class_ScriptEditor_method_get_current_editor:

- :ref:`ScriptEditorBase<class_ScriptEditorBase>` **get_current_editor** **(** **)** |const|

Returns the :ref:`ScriptEditorBase<class_ScriptEditorBase>` object that the user is currently editing.

----

.. _class_ScriptEditor_method_get_current_script:

- :ref:`Script<class_Script>` **get_current_script** **(** **)**

Returns a :ref:`Script<class_Script>` that is currently active in editor.

----

.. _class_ScriptEditor_method_get_open_script_editors:

- :ref:`Array<class_Array>` **get_open_script_editors** **(** **)** |const|

Returns an array with all :ref:`ScriptEditorBase<class_ScriptEditorBase>` objects which are currently open in editor.

----

.. _class_ScriptEditor_method_get_open_scripts:

- :ref:`Array<class_Array>` **get_open_scripts** **(** **)** |const|

Returns an array with all :ref:`Script<class_Script>` objects which are currently open in editor.

----

.. _class_ScriptEditor_method_goto_line:

- void **goto_line** **(** :ref:`int<class_int>` line_number **)**

Goes to the specified line in the current script.

----

.. _class_ScriptEditor_method_open_script_create_dialog:

- void **open_script_create_dialog** **(** :ref:`String<class_String>` base_name, :ref:`String<class_String>` base_path **)**

Opens the script create dialog. The script will extend ``base_name``. The file extension can be omitted from ``base_path``. It will be added based on the selected scripting language.

----

.. _class_ScriptEditor_method_register_syntax_highlighter:

- void **register_syntax_highlighter** **(** :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` syntax_highlighter **)**

Registers the :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` to the editor, the :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` will be available on all open scripts.

\ **Note:** Does not apply to scripts that are already opened.

----

.. _class_ScriptEditor_method_unregister_syntax_highlighter:

- void **unregister_syntax_highlighter** **(** :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` syntax_highlighter **)**

Unregisters the :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` from the editor.

\ **Note:** The :ref:`EditorSyntaxHighlighter<class_EditorSyntaxHighlighter>` will still be applied to scripts that are already opened.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
