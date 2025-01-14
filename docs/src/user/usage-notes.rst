General usage notes
===================

-  Run against **testing/staging clouds first**, verify that you are
   getting the expected results.

-  Use **different ``os_migrate_data_dir`` per project** you're
   authenticating to. OS Migrate works in project (tenant) scope most
   of the time. The data dir will be populated with the source
   project's exported resources, and should not be mixed with another
   project's resources.

   When you are changing ``os_migrate_src_auth`` or
   ``os_migrate_src_region_name`` parameters, make sure to also change
   ``os_migrate_data_dir``.

-  Use the **same version of OS Migrate for export and import**. We
   currently do not guarantee that data files are compatible across
   versions.

-  OS Migrate may not fit each use case out of the box. You can craft
   custom playbooks using the OS Migrate collection pieces (roles and
   modules) as building blocks.
