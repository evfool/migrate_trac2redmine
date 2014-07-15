migrate_trac2redmine
====================

This script is an updated version of the trac to redmine migration script. You should overwrite to lib/tasks/migrate_from_trac.rake.

Includes

 * This script supports Trac 1.0.1.
 * bugfixes
   * fixed time format issues with redmine (see redmine#14567)
   * attachments migration fixed (old redmine migrate script doesn't support Trac 1.0.1, looks for attachments in trac/attachments instead of trac/files/attachments)

TODO
 [ ] migrate custom ticket workflow
 [ ] migrate wiki syntax - patches from redmine#5035
   [ ] #XXXX format ticket references conversion to link
   [ ] = =, == ==, === === style headers conversion
   [ ] inline images conversion
   [ ] ticket list conversion
 [ ] do not import comments with "CommitTicketReference", as we will have those in the associated revisions view
 [ ] reverse_each for ticket changes to import them in chronological order
 [ ] check attachments import
