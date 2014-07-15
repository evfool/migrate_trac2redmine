migrate_trac2redmine
====================

This script is an updated version of the trac to redmine migration script. You should overwrite to lib/tasks/migrate_from_trac.rake.

Includes

 * This script supports Trac 1.0.1.
 * bugfixes
   * fixed time format issues with redmine (see redmine#14567)
   * attachments migration fixed (old redmine migrate script doesn't support Trac 1.0.1, looks for attachments in trac/attachments instead of trac/files/attachments)
