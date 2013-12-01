migrate_trac2redmine
====================

This script is patch of the redmine migration script. You should overwrite to lib/tasks/migrate_from_trac.rake.

# Future

 * This script support Trac 1.0.1.
 * support relation of wiki pages
 * some bug fixes
   * time format is wrong
   * can't get attachment files(old redmine migrate script doesn't support Trac 1.0.1)
