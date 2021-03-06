.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the MeshInstance.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_MeshInstance:

MeshInstance
============

**Inherits:** :ref:`GeometryInstance<class_geometryinstance>` **<** :ref:`VisualInstance<class_visualinstance>` **<** :ref:`Spatial<class_spatial>` **<** :ref:`Node<class_node>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

Node that instances meshes into a scenario.

Member Functions
----------------

+----------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`create_convex_collision<class_MeshInstance_create_convex_collision>` **(** **)**                                                                   |
+----------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`create_debug_tangents<class_MeshInstance_create_debug_tangents>` **(** **)**                                                                       |
+----------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`create_trimesh_collision<class_MeshInstance_create_trimesh_collision>` **(** **)**                                                                 |
+----------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Material<class_material>`  | :ref:`get_surface_material<class_MeshInstance_get_surface_material>` **(** :ref:`int<class_int>` surface **)** const                                     |
+----------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                             | :ref:`set_surface_material<class_MeshInstance_set_surface_material>` **(** :ref:`int<class_int>` surface, :ref:`Material<class_material>` material **)** |
+----------------------------------+----------------------------------------------------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_MeshInstance_mesh:

- :ref:`Mesh<class_mesh>` **mesh** - The :ref:`Mesh<class_mesh>` resource for the instance.

  .. _class_MeshInstance_skeleton:

- :ref:`NodePath<class_nodepath>` **skeleton** - :ref:`NodePath<class_nodepath>` to the :ref:`Skeleton<class_skeleton>` associated with the instance.


Description
-----------

MeshInstance is a node that takes a :ref:`Mesh<class_mesh>` resource and adds it to the current scenario by creating an instance of it. This is the class most often used to get 3D geometry rendered and can be used to instance a single :ref:`Mesh<class_mesh>` in many places. This allows to reuse geometry and save on resources. When a :ref:`Mesh<class_mesh>` has to be instanced more than thousands of times at close proximity, consider using a :ref:`MultiMesh<class_multimesh>` in a :ref:`MultiMeshInstance<class_multimeshinstance>` instead.

Member Function Description
---------------------------

.. _class_MeshInstance_create_convex_collision:

- void **create_convex_collision** **(** **)**

This helper creates a :ref:`StaticBody<class_staticbody>` child node with a :ref:`ConvexPolygonShape<class_convexpolygonshape>` collision shape calculated from the mesh geometry. It's mainly used for testing.

.. _class_MeshInstance_create_debug_tangents:

- void **create_debug_tangents** **(** **)**

This helper creates a :ref:`MeshInstance<class_meshinstance>` child node with gizmos at every vertex calculated from the mesh geometry. It's mainly used for testing.

.. _class_MeshInstance_create_trimesh_collision:

- void **create_trimesh_collision** **(** **)**

This helper creates a :ref:`StaticBody<class_staticbody>` child node with a :ref:`ConcavePolygonShape<class_concavepolygonshape>` collision shape calculated from the mesh geometry. It's mainly used for testing.

.. _class_MeshInstance_get_surface_material:

- :ref:`Material<class_material>` **get_surface_material** **(** :ref:`int<class_int>` surface **)** const

Returns the :ref:`Material<class_material>` for a surface of the :ref:`Mesh<class_mesh>` resource.

.. _class_MeshInstance_set_surface_material:

- void **set_surface_material** **(** :ref:`int<class_int>` surface, :ref:`Material<class_material>` material **)**

Sets the :ref:`Material<class_material>` for a surface of the :ref:`Mesh<class_mesh>` resource.


