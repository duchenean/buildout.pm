## Release 4.2.35-rc2

**Date:** 2025-12-03

### Package Updates

#### Products.PloneMeeting (4.2.28rc1 → 4.2.28rc3)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.15 → 4.2.16rc1)

*No changelog entries found.*

#### collective.iconifiedcategory (0.70 → 0.71)

#### Version 0.71 (2025-12-03)

- Avoid an error if category root folder does not exist
  [mpeeters]
- Optimized `upgrade_to_2107` (approved/to_approve).
  [chris-adam]

#### imio.pm.locales (4.2.32rc1 → 4.2.32rc3)

*No changelog entries found.*

#### plonetheme.imioapps (2.52 → 2.54)

#### Version 2.54 (2025-12-01)

- Make sure large images do not add horizontal scroll in tooltipsters.
  [gbastien]
- Fixed not used and mismatch use of `evenRowBackgroundColor` and
  `oddRowBackgroundColor`.
  [gbastien]

#### Version 2.53 (2025-08-21)

- URBBDC-3142: Change icon for Housing procedure.
  [aduchene, WBoudabous]

## Release 4.2.35-rc1

**Date:** 2025-11-05

### Package Updates

#### Products.PloneMeeting (4.2.27.4 → 4.2.28rc1)

*No changelog entries found.*

#### imio.helpers (1.3.3 → 1.3.7)

#### Version 1.3.7 (2025-11-05)

- Try to fix broken release.
  [gbastien]

#### Version 1.3.6 (2025-11-05)

- Try to fix broken release.
  [gbastien]

#### Version 1.3.5 (2025-11-05)

- Try to fix broken release.
  [gbastien]

#### Version 1.3.4 (2025-11-05)

- Adapted JS function `submitFormHelper`:

  - removed first parameter `form` that was not used;
  - manage CKeditor fields so it is correctly submitted.

  [gbastien]

#### collective.eeafaceted.batchactions (1.16.5 → 1.16.6)

#### Version 1.16.6 (2025-11-05)

- Added possibliity to use custom overlay configuration by setting
  `BaseBatchActionForm.overlay` attribute to `None`, in this case nothing is
  done and the overlay JS initialization must be done by an external package.
  [gbastien]

#### collective.iconifiedcategory (0.69 → 0.70)

#### Version 0.70 (2025-11-05)

- Fix invalid jQuery selector for default Title field filling
  [laulaz]
- Added "Approved?" column to the categorized elements table
  [chris-adam,sgeulette]
- Added cache on IconClickableColumn action view.
  [chris-adam]
- Added page reload possibility
  [sgeulette]
- Moved css pattern outside css generation view (`css.IconifiedCategory`)
  so it is reusable by an external package.
  [gbastien]

#### imio.pm.locales (4.2.31 → 4.2.32rc1)

*No changelog entries found.*

#### imio.zamqp.core (0.7 → 0.10)

#### Version 0.10 (2025-11-05)

- Commented unneeded code.
  [sgeulette]
- In `utils.highest_scan_id`, get `scan_id` from `brain` index instead metadata
  in case there is a desynchronization between index and metadata and we are
  sure we are re-using the same value as the one used to get
  the highest index value.
  [gbastien]

#### Version 0.9 (2024-02-12)

- Raised a ValueError in `utils.next_scan_id` when found highest id doesn't start with scan_type parameter.
  [sgeulette]

#### Version 0.8 (2024-02-12)

- Improved `utils.next_scan_id` to check if found highest id starts well with scan_type parameter.
  [sgeulette]
- Added gh actions for tests.
  [sgeulette]

## Release 4.2.34

**Date:** 2025-11-04

### Package Updates

#### Products.PloneMeeting (4.2.27 → 4.2.27.4)

#### Version 4.2.27.4 (2025-11-04)

- Fixed link to `iA.Vision`:

  - Check again if can link in `LinkWithVisionForm.update` and
    `LinkWithVisionForm.handle_apply`;
  - Do not fail to display error message if it contains unicode characters.

  [gbastien]

#### Version 4.2.27.3 (2025-11-03)

- Environment variable `MUNICIPALITY_ID` is actually `VISION_MUNICIPALITY_ID`.
  [gbastien]

#### Version 4.2.27.2 (2025-11-03)

- Take into acount environment variable `MUNICIPALITY_ID` to manage links
  to external applications.
  [gbastien]

#### Version 4.2.27.1 (2025-10-23)

- Fixed `ExternalView.show_section`, will not be available if
  `VISION_AUTH_USERNAME` is an empty string neither.
  [gbastien]

#### appy (1.0.18 → 1.0.20)

*No changelog entries found.*

#### collective.big.bang (1.0.3 → 1.0.4)

*No changelog entries found.*

## Release 4.2.34-rc9

**Date:** 2025-10-22

### Package Updates

#### Products.PloneMeeting (4.2.27rc2 → 4.2.27)

*No changelog entries found.*

#### imio.pm.locales (4.2.31rc1 → 4.2.31)

*No changelog entries found.*

## Release 4.2.34-rc8

**Date:** 2025-10-16

### Package Updates

#### Products.PloneMeeting (4.2.27rc1 → 4.2.27rc2)

#### Version 4.2.27.2 (2025-11-03)

- Take into acount environment variable `MUNICIPALITY_ID` to manage links
  to external applications.
  [gbastien]

#### imio.helpers (1.3.2 → 1.3.3)

#### Version 1.3.3 (2025-10-07)

- Added JS helper function `filterByName` that let filter a list of elements
  from a text input.
  [gbastien]

## Release 4.2.34-rc7

**Date:** 2025-10-13

### Package Updates

#### Products.PloneMeeting (4.2.26 → 4.2.27rc1)

#### Version 4.2.27.1 (2025-10-23)

- Fixed `ExternalView.show_section`, will not be available if
  `VISION_AUTH_USERNAME` is an empty string neither.
  [gbastien]

#### Version 4.2.27 (2025-10-22)

- Add 2026 holidays in profile.
  [aduchene]
- Fixed `MeetingItem.title_or_id` to return `portal_type's title` instead
  translated `portal_type` as now we do not translate `portal_type` anymore
  but use the `portal_type's title`.
  [gbastien]
- Manage item follow-up.
  [gbastien]
- Invalidate dashboard collection counter when a label is (un)selected.
  This is done only when the added/removed global or personal label is used in
  an enabled dashboard collection query.
  [gbastien]

#### imio.annex (2.24 → 2.25)

#### Version 2.25 (2025-10-13)

- For `DownloadAnnexesBatchActionForm` and `ConcatenateAnnexesBatchActionForm`,
  manage `MAX_TOTAL_SIZE` in method `_max_total_size` so it is easy to override
  and to manage functionnal usecases (like different max size depending
  on current user).
  [gbastien]
- Add `sort_on` parameter to `utils.get_annexes_to_print` so annexes can be sorted.
  [aduchene]

#### imio.pm.locales (4.2.30 → 4.2.31rc1)

#### Version 4.2.31 (2025-10-22)

- Added translations related to `item follow-up`.
  [gbastien]

## Release 4.2.34-rc6

**Date:** 2025-10-07

### Package Updates

#### Products.PloneMeeting (4.2.26rc1 → 4.2.26)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.14 → 4.2.15)

#### Version 4.2.15 (2025-10-07)

- Fixed `config.DEFAULT_FINANCE_ADVICES_TEMPLATE['initiative']` pattern,
  use `{by}` instead `{to}`.
  [gbastien]

#### imio.pm.locales (4.2.30rc1 → 4.2.30)

*No changelog entries found.*

## Release 4.2.34-rc5

**Date:** 2025-10-02

### Package Updates

#### Products.PloneMeeting (4.2.25 → 4.2.26rc1)

#### Version 4.2.26 (2025-10-07)

- Fixed `MeetingItem._updateAdvices` to avoid error when comparing `Dicts`
  `self.adviceIndex` and `old_adviceIndex` in case we have a `datetime.datetime`
  and a `None`.
  [gbastien]
- Display elements from external source `iA.Vision`, added form to be able
  to `link/unlink` elements from it as well.
  [gbastien]

#### imio.pm.locales (4.2.29 → 4.2.30rc1)

#### Version 4.2.30 (2025-10-07)

- Adapted footer translations to remove no more working links and simplify it.
  [gbastien]
- Added translations for `external` linked elements.
  [gbastien]

## Release 4.2.34-rc4

**Date:** 2025-09-29

### Package Updates

#### Products.PloneMeeting (4.2.24.3 → 4.2.25)

#### Version 4.2.25 (2025-09-26)

- Completed parameter `disable_autosearch_in` of `imio.webspellchecker` to
  include CSS class of input `go to item` on item view and `change item number`
  on meeting view.
  [gbastien]
- Display `voting group` in `MeetingConfig.orderedContacts` so we can detect
  easily for which held position it is configured.
  [gbastien]
- Added `MeetingConfig.labelsConfig` to be able to configure who can
  view/edit labels.
  [gbastien]
- Added parameter `extra_ctx={}` to `utils._base_extra_expr_ctx` to be able
  to pass extra context immediatelly without having to `dict.update` after.
  [gbastien]

#### Products.MeetingCommunes (4.2.13 → 4.2.14)

#### Version 4.2.14 (2025-09-26)

- Fixed the dashboard `Export` pod template that was not including advices
  because wrong parameter `dirfin` was passed to `get_all_items_dghv_with_advice`
  that expects a list of adviser uids for parameter `adviserUids=[]`.
  [gbastien]

#### imio.helpers (1.3.0 → 1.3.2)

#### Version 1.3.2 (2025-09-26)

- Improved `set.load_workflow_from_package` with default option `purge_workflow=True`.
  [sgeulette]
- Override `ftw.labels` portal_catalog index `labels` to add `EMPTY_STRING`
  value when no global label selected.
  [gbastien]

#### Version 1.3.1 (2025-08-26)

- Improved uninstall profile to permit install-base reinstall.
  [sgeulette]
- Add a parameter `extra_args=""` to `barcode.generate_barcode`
  to be able to pass extra arguments to the executable.
  [aduchene]
- Gracefully close the subprocess.Popen in `barcode.generate_barcode`
  to avoid "ResourceWarning: unclosed file..."
  [aduchene]
- Fixed obj_modified datetime that was sometimes None.
  [chris-adam]

#### collective.eeafaceted.batchactions (1.16.4 → 1.16.5)

#### Version 1.16.5 (2025-09-26)

- Added `PMLabelsBatchActionForm._filter_labels_vocabulary` to be able to filter
  selectable labels vocabulary.
  [gbastien]

#### imio.pm.locales (4.2.27 → 4.2.29)

#### Version 4.2.29 (2025-09-26)

- Cleanup.
  [gbastien]

#### Version 4.2.28 (2025-09-26)

- Added translations related to `MeetingConfig.labelsConfig`.
  [gbastien]

## Release 4.2.34-rc3

**Date:** 2025-09-18

### Package Updates

#### Products.PloneMeeting (4.2.24.2 → 4.2.24.3)

#### Version 4.2.24.3 (2025-09-04)

- Use median space to separate optional letters in `abstenu·e·s` of print_votes.
  [gbastien]

## Release 4.2.34-rc2

**Date:** 2025-08-28

### Package Updates

#### Products.PloneMeeting (4.2.27.1 → 4.2.24.2)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.15 → 4.2.13)

*No changelog entries found.*

#### imio.annex (2.25 → 2.24)

*No changelog entries found.*

#### imio.helpers (1.3.3 → 1.3.0)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.16.5 → 1.16.4)

*No changelog entries found.*

#### imio.pm.locales (4.2.31 → 4.2.27)

*No changelog entries found.*

## Release 4.2.34-rc10

**Date:** 2025-10-23

### Package Updates

#### Products.PloneMeeting (4.2.21rc1 → 4.2.27.1)

#### Version 4.2.27.1 (2025-10-23)

- Fixed `ExternalView.show_section`, will not be available if
  `VISION_AUTH_USERNAME` is an empty string neither.
  [gbastien]

#### Version 4.2.27 (2025-10-22)

- Add 2026 holidays in profile.
  [aduchene]
- Fixed `MeetingItem.title_or_id` to return `portal_type's title` instead
  translated `portal_type` as now we do not translate `portal_type` anymore
  but use the `portal_type's title`.
  [gbastien]
- Manage item follow-up.
  [gbastien]
- Invalidate dashboard collection counter when a label is (un)selected.
  This is done only when the added/removed global or personal label is used in
  an enabled dashboard collection query.
  [gbastien]

#### Version 4.2.26 (2025-10-07)

- Fixed `MeetingItem._updateAdvices` to avoid error when comparing `Dicts`
  `self.adviceIndex` and `old_adviceIndex` in case we have a `datetime.datetime`
  and a `None`.
  [gbastien]
- Display elements from external source `iA.Vision`, added form to be able
  to `link/unlink` elements from it as well.
  [gbastien]

#### Version 4.2.25 (2025-09-26)

- Completed parameter `disable_autosearch_in` of `imio.webspellchecker` to
  include CSS class of input `go to item` on item view and `change item number`
  on meeting view.
  [gbastien]
- Display `voting group` in `MeetingConfig.orderedContacts` so we can detect
  easily for which held position it is configured.
  [gbastien]
- Added `MeetingConfig.labelsConfig` to be able to configure who can
  view/edit labels.
  [gbastien]
- Added parameter `extra_ctx={}` to `utils._base_extra_expr_ctx` to be able
  to pass extra context immediatelly without having to `dict.update` after.
  [gbastien]

#### Version 4.2.24.3 (2025-09-04)

- Use median space to separate optional letters in `abstenu·e·s` of print_votes.
  [gbastien]

#### Version 4.2.24.2 (2025-08-28)

- Fixed `Migrate_To_4200._fixPODTemplatesInstructions` to manage
  `getMeetingNumber` to `meeting_number` replacement also in item related
  POD templates.
  [gbastien]
- Fixed `utils.sendMail` `translationMapping` to use correct title for
  `transitionTitle` and `meetingState/itemState`.
  This let's use new WF values in email notifications with correct WF
  transition and state title.
  [gbastien]
- Fixed `utils.sendMail`, return same result when `MeetingConfig.mailMode`
  is `test` or `enabled`.
  [gbastien]
- In `ItemDocumentGenerationHelperView.print_votes`, added possibility to
  use special character `|` in label so it will generate several different
  labels useable thru the `vote_label_pattern` parameter.
  [gbastien]
- Added parameter `is_voter=None` to `print_attendees` and
  `print_attendees_by_type` so it is possible to get attendees that are
  voters (`True`), non voters (`False`) or everybody (`None`).
  [gbastien]

#### Version 4.2.24.1 (2025-07-11)

- Fixed installation of `imio.webspellchecker` using helper
  `setuphandlers._installWebspellchecker`, need to prepend profile name with
  `profile-` when calling `portal_setup.runAllImportStepsFromProfile`.
  [gbastien]

#### Version 4.2.24 (2025-06-25)

- Added `imio.helpers.content.object_values` to `safe_utils` so it is available
  in TAL expressions and Python scripts.
  [gbastien]
- Fixed global labels not changeable using labels batch action form when
  `MeetingConfig.itemLabelsEditableByProposingGroupForever` is `True` by
  overriding `LabelsBatchActionForm._can_change_labels` to take into account
  our `PMLabeling.can_edit`.
  [gbastien]

#### Version 4.2.23.3 (2025-06-06)

- Make sure WSC is disabled in annex `content_category select2 widget` or
  it breaks `quickupload` of several annexes.
  [gbastien]

#### Version 4.2.23.2 (2025-06-06)

- Display `MeetingConfig.configGroup` on `meetingconfig_view` when listing
  POD templates and also in informations about "sendable to/sent to" on items
  (icons, actions).
  [gbastien]
- Added overlay CSS class `link-overlay-pm-info` to be used for overlays that
  may be closed safely when clicking outside of it.
  [gbastien]
- Fixed max width to `300px` for `copyGroups` column of items dashboards and
  `category` column of annexes table.
  [gbastien]
- Completed `test_pm_ItemAbsentsAndExcusedAndNonAttendees` to show that
  `@@display-meeting-item-not-present` works when current user can not access
  items for which assembly member is absent.
  [gbastien]

#### Version 4.2.23.1 (2025-05-28)

- Fixed `Migrate_To_4215._updateWFWriteMarginalNotesPermission` to only update
  items in state `presented`.
  [gbastien]

#### Version 4.2.23 (2025-05-27)

- Adapted call to `@@load_held_position_back_refs` to be able to pass a `limit`
  and so display more than 50 elements.
  [gbastien]
- Adpated step `_fixWSCConfigAndCleanBrokenAnnexes` of migration to 4215 to
  only disable `WSC` in `quickupload`.
  [gbastien]
- Use an `InAndOutWidget` for `MeetingConfig.usedVoteValues`,
  `MeetingConfig.firstLinkedVoteUsedVoteValues` and
  `MeetingConfig.nextLinkedVotesUsedVoteValues` so it is possible to change
  displayed order.
  [gbastien]
- When quick editing the `MeetingItem.internalNotes` field, do not make item
  `modified` as this field is somehow external to the item decision and more
  like a `post-it` field as it is the case for `labels`.
  [gbastien]
- Avoid overlays closing when using `WSC` in an editable field.
  [gbastien]
- Completed migration to 4215 with step `_updateWFWriteMarginalNotesPermission`
  to update item WF to manage `WriteMarginalNotes` given to `MeetingManager`
  when item is `presented`.
  [gbastien]
- Display `MeetingConfig.configGroup` everywhere necessary to avoid
  misinterpretation when several `MeetingConfigs` have same title in different
  `configGroups`.
  [gbastien]
- Fixed `MeetingItemWorkflowConditions.mayCorrect` and
  `MeetingItemWorkflowConditions._getLastValidationState` to use adaptable
  method `MeetingItem._getGroupManagingItem` instead
  `MeetingItem.getProposingGroup` when relevant or it is possible to correct
  to a validation state where group is empty because not using correct group.
  [gbastien]

#### Version 4.2.22 (2025-05-14)

- Completed migration to 4215 with step `_fixWSCConfigAndCleanBrokenAnnexes`
  to configure `WSC` and remove eventual broken annexes.
  [gbastien]
- Fixed error when editing votes on an item when a held position was disabled
  (actually when it had no more `usages`).
  [gbastien]

#### Products.MeetingCommunes (4.2.10 → 4.2.15)

#### Version 4.2.15 (2025-10-07)

- Fixed `config.DEFAULT_FINANCE_ADVICES_TEMPLATE['initiative']` pattern,
  use `{by}` instead `{to}`.
  [gbastien]

#### Version 4.2.14 (2025-09-26)

- Fixed the dashboard `Export` pod template that was not including advices
  because wrong parameter `dirfin` was passed to `get_all_items_dghv_with_advice`
  that expects a list of adviser uids for parameter `adviserUids=[]`.
  [gbastien]

#### Version 4.2.13 (2025-06-23)

- Fixed advice `item_transmitted_on_localized` date computation that was only
  considering `item_advice_states` from `MeetingConfig` but it can also be
  defined on the `organization` in which case it takes precedence.
  [gbastien]

#### Version 4.2.12 (2025-03-24)

- Added possibility to get generated finance advice for restapi in
  new key `deliberation_finance_advice`.
  [gbastien]

#### Version 4.2.11 (2025-03-11)

- Adapted `zcity` profile to use `contactsTemplates` from `examples_fr` profile.
  [gbastien]

#### imio.actionspanel (1.69 → 1.70)

#### Version 1.70 (2025-05-27)

- Avoid WSC (`webspellchecker`) closing the workflow transition comment overlay
  when applying correction.
  [gbastien]

#### imio.annex (2.24 → 2.25)

#### Version 2.25 (2025-10-13)

- For `DownloadAnnexesBatchActionForm` and `ConcatenateAnnexesBatchActionForm`,
  manage `MAX_TOTAL_SIZE` in method `_max_total_size` so it is easy to override
  and to manage functionnal usecases (like different max size depending
  on current user).
  [gbastien]
- Add `sort_on` parameter to `utils.get_annexes_to_print` so annexes can be sorted.
  [aduchene]

#### imio.helpers (1.2.2 → 1.3.3)

#### Version 1.3.3 (2025-10-07)

- Added JS helper function `filterByName` that let filter a list of elements
  from a text input.
  [gbastien]

#### Version 1.3.2 (2025-09-26)

- Improved `set.load_workflow_from_package` with default option `purge_workflow=True`.
  [sgeulette]
- Override `ftw.labels` portal_catalog index `labels` to add `EMPTY_STRING`
  value when no global label selected.
  [gbastien]

#### Version 1.3.1 (2025-08-26)

- Improved uninstall profile to permit install-base reinstall.
  [sgeulette]
- Add a parameter `extra_args=""` to `barcode.generate_barcode`
  to be able to pass extra arguments to the executable.
  [aduchene]
- Gracefully close the subprocess.Popen in `barcode.generate_barcode`
  to avoid "ResourceWarning: unclosed file..."
  [aduchene]
- Fixed obj_modified datetime that was sometimes None.
  [chris-adam]

#### Version 1.3.0 (2025-06-25)

- Fix Plone 6 JS registration & remove unused Plone 5.2 compatibility
  [laulaz]
- Added `registry-icons` view to display all available registry icons.
  [sgeulette]
- Added utils function is_valid_json.
  [chris-adam]
- Added Plone 6 uninstall profile.
  [chris-adam]

#### Version 1.2.4 (2025-06-06)

- Added JS function `expandCollapsible` that will expand a list of collapsibles
  (`toggleDetails`) passed as query parameter.
  [gbastien]
- Pinned `z3c.unconfigure` to `2.1` instead `3.0` as it breaks Plone6.0 tests.
  [gbastien]
- Overrided `collective.quickupload` JS function `_addSelection` to fix selected
  elements order (order was reversed).
  [gbastien]

#### Version 1.2.3 (2025-03-11)

- Improved `email.validate_email_address` to replace '""' in email.
  [sgeulette]
- Added Plone 6.1 version in buildout.
  [chris-adam]

#### imio.prettylink (1.22 → 1.23)

#### Version 1.23 (2025-06-06)

- Fixed tag title displaying `&apos;` because `html.escape` was done after
  replacing `'` by `&apos;`, now quote management is done after `html.escape`.
  [gbastien]

#### imio.pyutils (1.1.2 → 1.1.4)

#### Version 1.1.4 (2025-06-06)

- Fixed `IndexError` in `utils.get_ordinal_clusters` when `numbers=[]`.
  [gbastien]

#### Version 1.1.3 (2025-02-05)

- Improved datetime import in system to correct load_var evaluation.
  [sgeulette]

#### collective.behavior.talcondition (1.0a1 → 1.1.1)

#### Version 1.1.1 (2025-08-28)

- Added `checkPermission` from `portal_membership` to base expression context.
  [gbastien]

#### Version 1.1.0 (2025-05-05)

- Added Plone 6.1 version in buildout.
  [sgeulette]

#### collective.contact.plonegroup (1.53 → 1.55)

#### Version 1.55 (2025-08-28)

- Display settings label on settings form.
  [gbastien]

#### Version 1.54 (2025-06-25)

- Set `toggle_parent_active=true` when calling JS `toggleDetails` for opening
  an organization linked users and groups so the `[+]` turns to `[-]`.
  [gbastien]

#### collective.documentgenerator (3.44 → 3.45)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.16.2 → 1.16.5)

#### Version 1.16.5 (2025-09-26)

- Added `PMLabelsBatchActionForm._filter_labels_vocabulary` to be able to filter
  selectable labels vocabulary.
  [gbastien]

#### Version 1.16.4 (2025-06-25)

- Renamed `TransitionBatchActionForm.getAvailableTransitionsVoc` to
  `TransitionBatchActionForm.get_available_transitions_voc`.
  [gbastien]
- Moved `LabelsBatchActionForm` can change labels computation to
  `LabelsBatchActionForm._can_change_labels` so it is easy to override.
  [gbastien]

#### Version 1.16.3 (2025-05-08)

- Updated is_permitted function to check multiple permissions.
  [chris-adam]

#### collective.eeafaceted.z3ctable (2.27 → 2.29)

#### Version 2.29 (2025-06-06)

- Fixed `AbbrColumn` title displaying `&apos;` because `html.escape` was done
  after replacing `'` by `&apos;`, now `html.escape` is done before.
  [gbastien]

#### Version 2.28 (2024-09-18)

- Modified `columns.VocabularyColumn` column by handling multiple ignored_values.
  [sgeulette]
- Improved `colums.DateColumn` column by converting DateTime to compare correctly with ignored_values.
  [sgeulette]
- Python 3 compatibility.
  [gbastien]

#### collective.iconifiedcategory (0.68 → 0.69)

#### Version 0.69 (2025-06-23)

- Fixed typo in `Show preview?` french translation.
  [gbastien]

#### imio.pm.locales (4.2.25.1 → 4.2.31)

#### Version 4.2.31 (2025-10-22)

- Added translations related to `item follow-up`.
  [gbastien]

#### Version 4.2.30 (2025-10-07)

- Adapted footer translations to remove no more working links and simplify it.
  [gbastien]
- Added translations for `external` linked elements.
  [gbastien]

#### Version 4.2.29 (2025-09-26)

- Cleanup.
  [gbastien]

#### Version 4.2.28 (2025-09-26)

- Added translations related to `MeetingConfig.labelsConfig`.
  [gbastien]

#### Version 4.2.27 (2025-08-28)

- More accurate french translation for
  `advice_asked_again_and_historized_comments`.
  [gbastien]
- Adapted translation of votes form label field to explain use of `|`.
  [gbastien]

#### Version 4.2.26 (2025-06-06)

- More accurate french translations for
  `This attendee is marked as signatory for the ${number} following item(s)` and
  `This attendee is marked as ${not_present_type} for the ${number}
  following items (${clusters})`.
  [gbastien]

#### imio.webspellchecker (1.0b7 → 1.1)

#### Version 1.1 (2025-07-11)

- Fixed installation by renaming the `base` profile to `install-base` so it is
  no more alphabetically before `default`.
  Removed `metadata.xml` from the `install-base` profile.
  [gbastien, aduchene]

#### plonetheme.imioapps (2.51 → 2.52)

#### Version 2.52 (2025-06-25)

- URBBDC-3142: Add icon for EmptyBuildings procedure.
  [aduchene]
- SUP-44304. Change current state style in urban.
  [jchandelle]
- Fixed edit bar height some times smaller than buttons.
  [gbastien]

#### Products.CPUtils (1.25 → 1.26)

#### Version 1.26 (2025-08-28)

- Completed `object_info`, display `externalIdentifier` if exists.
  [gbastien]

## Release 4.2.34-rc1

**Date:** 2025-05-05

### Package Updates

#### Products.PloneMeeting (4.2.24.1 → 4.2.21rc1)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.13 → 4.2.10)

*No changelog entries found.*

#### imio.actionspanel (1.70 → 1.69)

*No changelog entries found.*

#### imio.helpers (1.3.0 → 1.2.2)

*No changelog entries found.*

#### imio.prettylink (1.23 → 1.22)

*No changelog entries found.*

#### imio.pyutils (1.1.4 → 1.1.2)

*No changelog entries found.*

#### collective.contact.plonegroup (1.54 → 1.53)

*No changelog entries found.*

#### collective.documentgenerator (3.45 → 3.44)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.16.4 → 1.16.2)

*No changelog entries found.*

#### collective.eeafaceted.z3ctable (2.29 → 2.27)

*No changelog entries found.*

#### collective.iconifiedcategory (0.69 → 0.68)

*No changelog entries found.*

#### imio.pm.locales (4.2.26 → 4.2.25.1)

*No changelog entries found.*

#### imio.webspellchecker (1.1 → 1.0b7)

*No changelog entries found.*

#### plonetheme.imioapps (2.52 → 2.51)

*No changelog entries found.*

## Release 4.2.33

**Date:** 2025-07-11

### Package Updates

#### Products.PloneMeeting (4.2.20rc2 → 4.2.24.1)

#### Version 4.2.24.1 (2025-07-11)

- Fixed installation of `imio.webspellchecker` using helper
  `setuphandlers._installWebspellchecker`, need to prepend profile name with
  `profile-` when calling `portal_setup.runAllImportStepsFromProfile`.
  [gbastien]

#### Version 4.2.24 (2025-06-25)

- Added `imio.helpers.content.object_values` to `safe_utils` so it is available
  in TAL expressions and Python scripts.
  [gbastien]
- Fixed global labels not changeable using labels batch action form when
  `MeetingConfig.itemLabelsEditableByProposingGroupForever` is `True` by
  overriding `LabelsBatchActionForm._can_change_labels` to take into account
  our `PMLabeling.can_edit`.
  [gbastien]

#### Version 4.2.23.3 (2025-06-06)

- Make sure WSC is disabled in annex `content_category select2 widget` or
  it breaks `quickupload` of several annexes.
  [gbastien]

#### Version 4.2.23.2 (2025-06-06)

- Display `MeetingConfig.configGroup` on `meetingconfig_view` when listing
  POD templates and also in informations about "sendable to/sent to" on items
  (icons, actions).
  [gbastien]
- Added overlay CSS class `link-overlay-pm-info` to be used for overlays that
  may be closed safely when clicking outside of it.
  [gbastien]
- Fixed max width to `300px` for `copyGroups` column of items dashboards and
  `category` column of annexes table.
  [gbastien]
- Completed `test_pm_ItemAbsentsAndExcusedAndNonAttendees` to show that
  `@@display-meeting-item-not-present` works when current user can not access
  items for which assembly member is absent.
  [gbastien]

#### Version 4.2.23.1 (2025-05-28)

- Fixed `Migrate_To_4215._updateWFWriteMarginalNotesPermission` to only update
  items in state `presented`.
  [gbastien]

#### Version 4.2.23 (2025-05-27)

- Adapted call to `@@load_held_position_back_refs` to be able to pass a `limit`
  and so display more than 50 elements.
  [gbastien]
- Adpated step `_fixWSCConfigAndCleanBrokenAnnexes` of migration to 4215 to
  only disable `WSC` in `quickupload`.
  [gbastien]
- Use an `InAndOutWidget` for `MeetingConfig.usedVoteValues`,
  `MeetingConfig.firstLinkedVoteUsedVoteValues` and
  `MeetingConfig.nextLinkedVotesUsedVoteValues` so it is possible to change
  displayed order.
  [gbastien]
- When quick editing the `MeetingItem.internalNotes` field, do not make item
  `modified` as this field is somehow external to the item decision and more
  like a `post-it` field as it is the case for `labels`.
  [gbastien]
- Avoid overlays closing when using `WSC` in an editable field.
  [gbastien]
- Completed migration to 4215 with step `_updateWFWriteMarginalNotesPermission`
  to update item WF to manage `WriteMarginalNotes` given to `MeetingManager`
  when item is `presented`.
  [gbastien]
- Display `MeetingConfig.configGroup` everywhere necessary to avoid
  misinterpretation when several `MeetingConfigs` have same title in different
  `configGroups`.
  [gbastien]
- Fixed `MeetingItemWorkflowConditions.mayCorrect` and
  `MeetingItemWorkflowConditions._getLastValidationState` to use adaptable
  method `MeetingItem._getGroupManagingItem` instead
  `MeetingItem.getProposingGroup` when relevant or it is possible to correct
  to a validation state where group is empty because not using correct group.
  [gbastien]

#### Version 4.2.22 (2025-05-14)

- Completed migration to 4215 with step `_fixWSCConfigAndCleanBrokenAnnexes`
  to configure `WSC` and remove eventual broken annexes.
  [gbastien]
- Fixed error when editing votes on an item when a held position was disabled
  (actually when it had no more `usages`).
  [gbastien]

#### Version 4.2.21 (2025-05-08)

- Removed useless index `is_default_page` from item templates tree query.
  [gbastien]
- Fixed migration to 4215 by re-applying `collective.documentgenerator` related
  customizations (`portal_type`, `viewlet`) as it is reinstalled by
  `collective.contact.core` upgrade during install of dependency `imio.fpaudit`.
  [gbastien]
- When cloning an item, re-apply auto committees in case configuration changed.
  [gbastien]

#### Products.MeetingCommunes (4.2.10 → 4.2.13)

#### Version 4.2.13 (2025-06-23)

- Fixed advice `item_transmitted_on_localized` date computation that was only
  considering `item_advice_states` from `MeetingConfig` but it can also be
  defined on the `organization` in which case it takes precedence.
  [gbastien]

#### Version 4.2.12 (2025-03-24)

- Added possibility to get generated finance advice for restapi in
  new key `deliberation_finance_advice`.
  [gbastien]

#### Version 4.2.11 (2025-03-11)

- Adapted `zcity` profile to use `contactsTemplates` from `examples_fr` profile.
  [gbastien]

#### imio.actionspanel (1.69 → 1.70)

#### Version 1.70 (2025-05-27)

- Avoid WSC (`webspellchecker`) closing the workflow transition comment overlay
  when applying correction.
  [gbastien]

#### imio.helpers (1.2.2 → 1.3.0)

#### Version 1.3.0 (2025-06-25)

- Fix Plone 6 JS registration & remove unused Plone 5.2 compatibility
  [laulaz]
- Added `registry-icons` view to display all available registry icons.
  [sgeulette]
- Added utils function is_valid_json.
  [chris-adam]
- Added Plone 6 uninstall profile.
  [chris-adam]

#### Version 1.2.4 (2025-06-06)

- Added JS function `expandCollapsible` that will expand a list of collapsibles
  (`toggleDetails`) passed as query parameter.
  [gbastien]
- Pinned `z3c.unconfigure` to `2.1` instead `3.0` as it breaks Plone6.0 tests.
  [gbastien]
- Overrided `collective.quickupload` JS function `_addSelection` to fix selected
  elements order (order was reversed).
  [gbastien]

#### Version 1.2.3 (2025-03-11)

- Improved `email.validate_email_address` to replace '""' in email.
  [sgeulette]
- Added Plone 6.1 version in buildout.
  [chris-adam]

#### imio.prettylink (1.22 → 1.23)

#### Version 1.23 (2025-06-06)

- Fixed tag title displaying `&apos;` because `html.escape` was done after
  replacing `'` by `&apos;`, now quote management is done after `html.escape`.
  [gbastien]

#### imio.pyutils (1.1.2 → 1.1.4)

#### Version 1.1.4 (2025-06-06)

- Fixed `IndexError` in `utils.get_ordinal_clusters` when `numbers=[]`.
  [gbastien]

#### Version 1.1.3 (2025-02-05)

- Improved datetime import in system to correct load_var evaluation.
  [sgeulette]

#### collective.contact.plonegroup (1.52 → 1.54)

#### Version 1.54 (2025-06-25)

- Set `toggle_parent_active=true` when calling JS `toggleDetails` for opening
  an organization linked users and groups so the `[+]` turns to `[-]`.
  [gbastien]

#### Version 1.53 (2025-05-05)

- Corrected bugs in `settings.validateSettings`.
  [sgeulette]
- Include user email in addition to id in `@@display-group-users`
  so we have `Fullname (user_id, user@email)` for `Managers`.
  [gbastien]

#### collective.documentgenerator (3.44 → 3.45)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.16.2 → 1.16.4)

#### Version 1.16.4 (2025-06-25)

- Renamed `TransitionBatchActionForm.getAvailableTransitionsVoc` to
  `TransitionBatchActionForm.get_available_transitions_voc`.
  [gbastien]
- Moved `LabelsBatchActionForm` can change labels computation to
  `LabelsBatchActionForm._can_change_labels` so it is easy to override.
  [gbastien]

#### Version 1.16.3 (2025-05-08)

- Updated is_permitted function to check multiple permissions.
  [chris-adam]

#### collective.eeafaceted.z3ctable (2.27 → 2.29)

#### Version 2.29 (2025-06-06)

- Fixed `AbbrColumn` title displaying `&apos;` because `html.escape` was done
  after replacing `'` by `&apos;`, now `html.escape` is done before.
  [gbastien]

#### Version 2.28 (2024-09-18)

- Modified `columns.VocabularyColumn` column by handling multiple ignored_values.
  [sgeulette]
- Improved `colums.DateColumn` column by converting DateTime to compare correctly with ignored_values.
  [sgeulette]
- Python 3 compatibility.
  [gbastien]

#### collective.iconifiedcategory (0.68 → 0.69)

#### Version 0.69 (2025-06-23)

- Fixed typo in `Show preview?` french translation.
  [gbastien]

#### imio.pm.locales (4.2.24.2 → 4.2.26)

#### Version 4.2.26 (2025-06-06)

- More accurate french translations for
  `This attendee is marked as signatory for the ${number} following item(s)` and
  `This attendee is marked as ${not_present_type} for the ${number}
  following items (${clusters})`.
  [gbastien]

#### Version 4.2.25 (2025-05-05)

- Added translation for `icon_help_isAcceptableOutOfMeeting`.
  [gbastien]
- Added translations for `MeetingConfig.customAdvisers`
  new `is_delay_calendar_days` column related functionality.
  [gbastien]

#### imio.webspellchecker (1.0b7 → 1.1)

#### Version 1.1 (2025-07-11)

- Fixed installation by renaming the `base` profile to `install-base` so it is
  no more alphabetically before `default`.
  Removed `metadata.xml` from the `install-base` profile.
  [gbastien, aduchene]

#### plonemeeting.restapi (2.8 → 2.9)

#### Version 2.9 (2025-05-05)

- SUP-43789: Fixed an issue with `utils.clean_html` when the ending tag </p> was not at the end of the content string.
  [aduchene]

#### plonetheme.imioapps (2.51 → 2.52)

#### Version 2.52 (2025-06-25)

- URBBDC-3142: Add icon for EmptyBuildings procedure.
  [aduchene]
- SUP-44304. Change current state style in urban.
  [jchandelle]
- Fixed edit bar height some times smaller than buttons.
  [gbastien]

## Release 4.2.33-rc2

**Date:** 2025-04-24

### Package Updates

#### Products.PloneMeeting (4.2.20rc1 → 4.2.20rc2)

*No changelog entries found.*

#### imio.pm.locales (4.2.24.1 → 4.2.24.2)

*No changelog entries found.*

## Release 4.2.33-rc1

**Date:** 2025-04-16

### Package Updates

#### Products.PloneMeeting (4.2.19 → 4.2.20rc1)

#### Version 4.2.20 (2025-05-05)

- When using `MeetingItem.otherMeetingConfigsClonableToFields`, make sure if
  field is empty, the resulting item field `mimetype` is correctly set to
  `text/html` (was `text/plain` resulting in broken `quick edit`).
  [gbastien]
- Adapted `MeetingItemWorkflowConditions.mayPresent` so an item that
  `isAcceptableOutOfMeeting` can not be presented into a meeting.
  [gbastien]
- Use another translation for `isAcceptableOutOfMeeting` pretty link icon title.
  [gastien]
- Fixed `Migrate_To_4211._updateDataRelatedToToolPloneMeetingSimplification`
  that was broken since `imio.fpaudit` that reinstalls
  `collective.documentgenerator` and breaks our custom
  `ConfigurablePODTemplate` portal_type.
  [gbastien]
- Added column `is_delay_calendar_days` to `MeetingConfig.customAdvisers`,
  when set to `1` advice delay will be computed in calendar days.
  [gbastien]
- Renamed `@@advice_delay_change_form` to `@@advice-delay-change-form`.
  Fixed `UnicodeDecodeError` when `delay_label` contains special characters.
  [gbastien]
- Avoid add/edit advice popup closing when using WSC.
  [gbastien]
- When sending email notifications, prepend `MeetingConfig.configGroup`
  `full_label` when used and several `MeetingConfigs` have same title
  so we know from which `MeetingConfig` the notification is sent.
  [gbastien]

#### Products.MeetingCommunes (4.2.12 → 4.2.10)

*No changelog entries found.*

#### imio.pm.locales (4.2.24 → 4.2.24.1)

*No changelog entries found.*

## Release 4.2.32

**Date:** 2025-05-26

### Package Updates

#### Products.PloneMeeting (4.2.13rc2 → 4.2.19)

#### Version 4.2.19 (2025-04-02)

- Fixed MeetingItem `actions_panel` caching that could display WF transitions
  actually not available. Transition could not be triggered anyway.
  [gbastien]
- In `ToolPloneMeeting.update_all_local_roles` only display the `Done.` message
  if `redirect=True` so it is not displayed in the dashboard batch action.
  [gbastien]
- Fixed `BaseCopyGroupsVocabulary` that could break because of several terms
  with same value when `copyGroups` and `restrictedCopyGroups` were used.
  [gbastien]

#### Version 4.2.18 (2025-03-24)

- Fixed do not display `MeetingConfig` title in page title
  if faceted context is a `meeting`.
  [gbastien]
- Make `MeetingConfig.lastMeetingNumber` required so it can never be `None`.
  [gbastien]
- Adapted POD template mailing list functionnality so the list of
  email addresses to which the mailing list will be sent to is display when
  hovering the mailing list and also displayed in the confirmation message when
  the mail has been sent.
  [gbastien]
- Adapted `getGroupsInCharge` item catalog index to not include
  auto groups in charge as it is stored on the item.
  Make groups in charge batch action available to `MeetingManagers` when using
  `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup` or
  `MeetingConfig.includeGroupsInChargeDefinedOnCategory`.
  [gbastien]

#### Version 4.2.17 (2025-03-17)

- Make `test_pm_json_collections_count` more robust by disabling every workflow
  adaptations so a custom profile will not enable a `DashboardCollection`
  that is using a counter.
  [gbastien]
- In `MeetingItem.getGivenAdvices` use `toLocalizedTime`
  from `@@plone` instead python script.
  [gbastien]
- Do not close add/edit annex overlay when clicking outside of it.
  [gbastien]
- When duplicating an item and using groups in charge on the category, make sure
  the new item uses groups in charge defined on the category and not original
  item groups in charge in case configuration was changed on the category.
  Make also sure that when an item is sent to another `MeetingConfig`, groups
  in charge defined on destination category are correctly applied on new item.
  On the `MeetingItem` view, do not `includeAuto=True` for groups in charge,
  display really stored groups in charge.
  [gbastien]

#### Version 4.2.16 (2025-03-11)

- Fixed `@@json_collections_count` caching invalidation for collections using
  a criterion refering to current connected user.
  [gbastien]
- Added new advice type `Positive after modification`.
  [gbastien]
- Added `fplog` when inserting/removing item from meeting.
  [gbastien]
- When not using the `decided` meeting workflow state,
  meeting is always considered `decided`.
  [gbastien]
- Optimized `MeetingItem.getMeetingToInsertIntoWhenNoCurrentMeetingObject`
  cachekey to not cache per item but per `MeetingConfig` and only consider
  `preferredMeeting`.
  [gbastien]
- On item templates and recurring items make sure every active delay aware
  advisers are displayed, ignore the `for_item_created_from` information.
  [gbastien]
- Fixed POD template mailing list containing a quote (') was breaking JS.
  [gbastien]
- Added logging when reindexing every items icon color
  when changed in `MeetingConfig`.
  [gbastien]

#### Version 4.2.15 (2025-02-06)

- Optimized `Meeting._update_using_groups_local_roles` that may be called on
  every existing meetings when saving several organizations in parameter
  `MeetingConfig.usingGroups`.
  This leaded to several minutes to save the `MeetingConfig`.
  [gbastien]
- Added confirmation dialog when clicking on `Send to other MeetingConfig`
  button as this will send the item to another `MeetingConfig` immediately.
  [gbastien]
- For `Delete whole meeting` confirm dialog message,
  use specific message `plonemeeting_delete_meeting_confirm_message`.
  [gbastien]
- In `PloneGroupSettingsOrganizationsValidator` display full `MeetingConfig`
  title (including `configGroup` label) in case several `MeetingConfigs` with
  same title exist in different config groups.
  [gbastien]

#### Version 4.2.14 (2025-02-03)

- Fixed an issue when `MeetingItem.proposingGroupWithGroupInCharge` is used in a
  `MeetingConfig` but not in another one when an item is sent to it.
  [aduchene]
- Prevent to unselect an organization in plonegroup that
  is used by `MeetingConfig.usingGroups`.
  [gbastien]
- Fixed `otherMeetingConfigsClonableToFieldXXX` field management when it is
  empty, it was not emptying the value on new item, now it is the case except
  for `title` that can not be empty.
  [gbastien]
- Make `MeetingItem.marginalNotes` field editable by `MeetingManagers` when item
  is `presented` (before it was when item was `itemfrozen`) so votes are also
  editable when item is `presented` as it relies on same permission
  `WriteMarginalNotes` that we should change name to a more generic name like
  `WriteClosedMeetingMeetingManagersReservedFields`.
  [gbastien]
- Renamed `_get_default_attendees` to `get_default_attendees`,
  `_get_default_signatories` to `get_default_signatories` and
  `_get_default_voters` to `_get_default_voters` and added it to `safe_utils`
  so it may be used in restricted python code.
  [gbastien]
- Added parameter `signatories={}` to `BaseDGHV.print_signatories_by_position`
  to be able to pass a dict of arbitrary held positions to render as signatures.
  This is useful for printing default signatories for example when we do
  not want to use signatories defined on context (item or meeting).
  [gbastien]
- Fixed `PMAttendeeRedefinePositionTypesVocabulary` that did not render default
  value term of `IRedefineAttendeePosition.position_type` correctly when it was
  not in the base vocabulary.
  [gbastien]
- Display `MeetingConfig` title in page title (displayed in web browser tab)
  on faceted contexts (dashboard and in configuration) so user knows where he is
  when using several tabs.
  [gbastien]
- Fixed `PMCategorizedObjectAdapter.can_view` when managing not viewable items
  because it could lead to unwanted users having access to some annexes by
  accessing it's URL directly.
  [gbastien]
- Make sure annexes only previewable (not downloadable) are not selectable
  when duplicating an item, exporting it to PDF or exporting annexes to Zip.
  [gbastien]
- Renamed `Migrator.updateItemFilters` to `Migrator.update_faceted_filters` and
  `Migrator.cleanUsedItemAttributes` to `Migrator.update_used_attrs` and
  manage `to_add/to_remove/to_replace` for each methods.
  [gbastien]
- In the votes editing form, highlight the value selected by the radio button
  as in some application the radio button is before or after the value.
  Renamed forms `item_encode_votes_form` to `item-encode-votes-form` and
  `item_encode_secret_votes_form` to `item-encode-secret-votes-form`.
  [gbastien]
- Prevent closing overlays when clicking outside it if it contains a form
  so we avoid losing encoded data if user clicked outside by mistake.
  [gbastien]
- Make `return_to_proposing_group` with validations more standalone by
  generating everything based on the `MeetingConfig.itemWFValidationLevels`.
  [gbastien]

#### Products.MeetingCommunes (4.2.9 → 4.2.12)

#### Version 4.2.12 (2025-03-24)

- Added possibility to get generated finance advice for restapi in
  new key `deliberation_finance_advice`.
  [gbastien]

#### Version 4.2.11 (2025-03-11)

- Adapted `zcity` profile to use `contactsTemplates` from `examples_fr` profile.
  [gbastien]

#### Version 4.2.10 (2024-11-07)

- Adapted `zcity` profile so `annexeDecisionToSign` and `annexeDecisionSigned`
  annex types are already configured by default.
  [gbastien]

#### imio.actionspanel (1.68 → 1.69)

#### Version 1.69 (2025-02-03)

- Prevent closing the workflow transition comment overlay when clicking outside
  it so we avoid losing comment in case user click outside by mistake.
  [gbastien]

#### imio.annex (2.23 → 2.24)

#### Version 2.24 (2025-02-03)

- Fixed `DownloadAnnexesBatchActionForm` to not download annexes that are only
  previewable (annexes for which `show_download` is `False`).
  [gbastien]

#### imio.helpers (1.0.0rc3 → 1.2.2)

#### Version 1.2.2 (2025-02-06)

- Added parameters `ask_confirm=false, confirm_msg='are_you_sure'` to
  JS function `callViewAndReload` so it is possible to have a
  confirmation dialog to execute the action or not.
  [gbastien]

#### Version 1.2.1 (2025-01-20)

- Improved `emailer.send_email` to take into account 3.10.12 python bug.
  [sgeulette]
- Removed ipython
  [sgeulette]

#### Version 1.2.0 (2024-12-19)

- Added new parameter to `batching.batch_get_keys`.
  [sgeulette]

#### Version 1.1.0 (2024-10-02)

- Imported batch_delete_files from imio.pyutils if someone is yet using it from here.
  [sgeulette]
- batch is considered finished if no batching.
  [sgeulette]

#### Version 1.0.1 (2024-09-18)

- Generated universal wheel version.
  [sgeulette]

#### Version 1.0.0rc4 (2024-07-08)

- Added "empty" variables to handle empty indexes searches.
  [sgeulette]

#### imio.pyutils (1.0.3 → 1.1.2)

#### Version 1.1.2 (2024-12-19)

- Improved `batching.batch_delete_files`.
  [sgeulette]

#### Version 1.1.1 (2024-09-18)

- Generated universal wheel version.
  [sgeulette]

#### Version 1.1.0 (2024-09-17)

- Added `utils.add_key_if_value` to add a key in a dic only if value or is not None.
  [sgeulette]
- Moved `batching.batch_delete_files` from imio.helpers to be used commonly.
  [sgeulette]

#### Version 1.0.4 (2024-06-11)

- Blacked files.
  [sgeulette]
- Added `system.post_request` to send a POST request.
  [sgeulette]

#### collective.contact.core (1.39 → 1.43.1)

#### Version 1.43.1 (2025-02-28)

- Added libjpeg8 for Pillow install in gha.
  [sgeulette]
- Added libbz2-dev for feedparser install in gha.
  [sgeulette]
- Moved include package `imio.fpaudit` from `testing.zcml` to `configure.zcml`.
  [gbastien]

#### Version 1.43.0 (2025-02-20)

- Added audit_access function, called at some places, to log contact access.
  [sgeulette]

#### Version 1.42.0 (2023-09-13)

- Set mail index lowercase.
  [sgeulette]

#### Version 1.41 (2023-09-07)

- Improved date ranges.
  [sgeulette]

#### Version 1.40 (2023-07-20)

- Added plone.app.iterate dependency.
  [sgeulette]
- Replaced subscribers grok declaration by zcml
  [sgeulette]
- Added subscribers docstrings
  [sgeulette]
- fix: [DMS-949] min & max for start_date, end_date
  [bleybaert]

#### collective.contact.plonegroup (1.51 → 1.52)

#### Version 1.52 (2025-02-06)

- Added parameter `verify_group_exist=True` to `utils.get_plone_groups`.
  When set to `False`, it will not get the real Plone group object to check
  if it exist when using `ids_only=True`. In this case it is much faster.
  [gbastien]

#### collective.documentgenerator (3.43 → 3.44)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.15 → 1.16.2)

#### Version 1.16.2 (2025-02-28)

- Overrided `Form.__call__` to not render if request reponse status
  is 204 (No content) as it is already the case when response status is 302 or
  the portal message is not displayed after faceted refresh because
  it was already displayed on the closing form.
  [gbastien]
- Added Attributes in modified call to specify which attribute has been modified.
  [cadam, sgeulette]
- Corrected typo
  [sgeulette]

#### Version 1.16.1 (2025-02-03)

- Check again `self.do_apply` in `BaseBatchActionForm.handleApply` to avoid
  nasty behaviors.
  [gbastien]

#### Version 1.16.0 (2024-12-19)

- Overrided `ContactBaseBatchActionForm.available` method to handle anonymous
  search correctly.
  [sgeulette]

#### collective.iconifiedcategory (0.67 → 0.68)

#### Version 0.68 (2025-02-03)

- Fixed `CategorizedObjectAdapter.can_view` default implementation that was
  checking `View` permission on context but we need to check on
  `categorized_obj` as permissions could be different.
  [gbastien]

#### imio.pm.locales (4.2.20.4 → 4.2.24)

#### Version 4.2.24 (2025-03-24)

- Added translation for `pt_mailing_will_be_sent_to`.
  [gbastien]

#### Version 4.2.23 (2025-03-11)

- Added translations for `Change committees` batch action.
  [gbastien]
- Added translations for new advice type `Positive after modification`.
  [gbastien]

#### Version 4.2.22 (2025-02-03)

- Added translations for `can_not_unselect_plone_group_meetingconfig`.
  [gbastien]
- Added translations related to only previewable annexes not duplicated.
  [gbastien]
- Adapted `return_to_proposing_group` with validation WFA related translations.
  Removed no more used `returned_to_proposing_group_with_validation_state`.
  [gbastien]
- Overrided `collective.iconifiedcategory` translation of
  `Show preview description.` to be more specific regarding `PloneMeeting`.
  [gbastien]

#### Version 4.2.21 (2024-11-07)

- Removed unused translation `restricted_copy_groups_item_descr`.
  [gbastien]
- Added translations for `PloneMeeting_label_emergencyMotivation`.
  [gbastien]

#### plonetheme.imioapps (2.50 → 2.51)

#### Version 2.51 (2025-03-11)

- If current URL contains `imio-acceptation`,
  highlight `portal-header` (turn it red).
  [gbastien]

## Release 4.2.32-test2

**Date:** 2024-11-14

### Package Updates

#### Products.PloneMeeting (4.2.13rc1 → 4.2.13rc2)

*No changelog entries found.*

#### imio.pm.locales (4.2.20.3 → 4.2.20.4)

*No changelog entries found.*

## Release 4.2.32-test

**Date:** 2024-11-12

### Package Updates

#### Products.PloneMeeting (4.2.14rc2 → 4.2.13rc1)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.10 → 4.2.9)

*No changelog entries found.*

#### imio.pm.locales (4.2.20.4 → 4.2.20.3)

*No changelog entries found.*

## Release 4.2.32-rc3

**Date:** 2025-01-10

### Package Updates

#### Products.PloneMeeting (4.2.14rc1 → 4.2.14rc2)

*No changelog entries found.*

## Release 4.2.32-rc2

**Date:** 2024-12-17

### Package Updates

#### Products.PloneMeeting (4.2.13rc3 → 4.2.14rc1)

#### Version 4.2.14 (2025-02-03)

- Fixed an issue when `MeetingItem.proposingGroupWithGroupInCharge` is used in a
  `MeetingConfig` but not in another one when an item is sent to it.
  [aduchene]
- Prevent to unselect an organization in plonegroup that
  is used by `MeetingConfig.usingGroups`.
  [gbastien]
- Fixed `otherMeetingConfigsClonableToFieldXXX` field management when it is
  empty, it was not emptying the value on new item, now it is the case except
  for `title` that can not be empty.
  [gbastien]
- Make `MeetingItem.marginalNotes` field editable by `MeetingManagers` when item
  is `presented` (before it was when item was `itemfrozen`) so votes are also
  editable when item is `presented` as it relies on same permission
  `WriteMarginalNotes` that we should change name to a more generic name like
  `WriteClosedMeetingMeetingManagersReservedFields`.
  [gbastien]
- Renamed `_get_default_attendees` to `get_default_attendees`,
  `_get_default_signatories` to `get_default_signatories` and
  `_get_default_voters` to `_get_default_voters` and added it to `safe_utils`
  so it may be used in restricted python code.
  [gbastien]
- Added parameter `signatories={}` to `BaseDGHV.print_signatories_by_position`
  to be able to pass a dict of arbitrary held positions to render as signatures.
  This is useful for printing default signatories for example when we do
  not want to use signatories defined on context (item or meeting).
  [gbastien]
- Fixed `PMAttendeeRedefinePositionTypesVocabulary` that did not render default
  value term of `IRedefineAttendeePosition.position_type` correctly when it was
  not in the base vocabulary.
  [gbastien]
- Display `MeetingConfig` title in page title (displayed in web browser tab)
  on faceted contexts (dashboard and in configuration) so user knows where he is
  when using several tabs.
  [gbastien]
- Fixed `PMCategorizedObjectAdapter.can_view` when managing not viewable items
  because it could lead to unwanted users having access to some annexes by
  accessing it's URL directly.
  [gbastien]
- Make sure annexes only previewable (not downloadable) are not selectable
  when duplicating an item, exporting it to PDF or exporting annexes to Zip.
  [gbastien]
- Renamed `Migrator.updateItemFilters` to `Migrator.update_faceted_filters` and
  `Migrator.cleanUsedItemAttributes` to `Migrator.update_used_attrs` and
  manage `to_add/to_remove/to_replace` for each methods.
  [gbastien]
- In the votes editing form, highlight the value selected by the radio button
  as in some application the radio button is before or after the value.
  Renamed forms `item_encode_votes_form` to `item-encode-votes-form` and
  `item_encode_secret_votes_form` to `item-encode-secret-votes-form`.
  [gbastien]
- Prevent closing overlays when clicking outside it if it contains a form
  so we avoid losing encoded data if user clicked outside by mistake.
  [gbastien]
- Make `return_to_proposing_group` with validations more standalone by
  generating everything based on the `MeetingConfig.itemWFValidationLevels`.
  [gbastien]

## Release 4.2.32-rc1

**Date:** 2024-12-05

### Package Updates

#### Products.PloneMeeting (4.2.19 → 4.2.13rc3)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.12 → 4.2.10)

*No changelog entries found.*

#### imio.actionspanel (1.69 → 1.68)

*No changelog entries found.*

#### imio.annex (2.24 → 2.23)

*No changelog entries found.*

#### imio.helpers (1.2.2 → 1.0.0rc3)

*No changelog entries found.*

#### imio.pyutils (1.1.2 → 1.0.3)

*No changelog entries found.*

#### collective.contact.core (1.43.1 → 1.39)

*No changelog entries found.*

#### collective.contact.plonegroup (1.52 → 1.51)

*No changelog entries found.*

#### collective.documentgenerator (3.44 → 3.43)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.16.2 → 1.15)

*No changelog entries found.*

#### collective.iconifiedcategory (0.68 → 0.67)

*No changelog entries found.*

#### imio.pm.locales (4.2.24 → 4.2.20.4)

*No changelog entries found.*

#### plonetheme.imioapps (2.51 → 2.50)

*No changelog entries found.*

## Release 4.2.32-municipalia2025

**Date:** 2025-04-15

### Package Updates

#### Products.PloneMeeting (4.2.16 → 4.2.19)

#### Version 4.2.19 (2025-04-02)

- Fixed MeetingItem `actions_panel` caching that could display WF transitions
  actually not available. Transition could not be triggered anyway.
  [gbastien]
- In `ToolPloneMeeting.update_all_local_roles` only display the `Done.` message
  if `redirect=True` so it is not displayed in the dashboard batch action.
  [gbastien]
- Fixed `BaseCopyGroupsVocabulary` that could break because of several terms
  with same value when `copyGroups` and `restrictedCopyGroups` were used.
  [gbastien]

#### Version 4.2.18 (2025-03-24)

- Fixed do not display `MeetingConfig` title in page title
  if faceted context is a `meeting`.
  [gbastien]
- Make `MeetingConfig.lastMeetingNumber` required so it can never be `None`.
  [gbastien]
- Adapted POD template mailing list functionnality so the list of
  email addresses to which the mailing list will be sent to is display when
  hovering the mailing list and also displayed in the confirmation message when
  the mail has been sent.
  [gbastien]
- Adapted `getGroupsInCharge` item catalog index to not include
  auto groups in charge as it is stored on the item.
  Make groups in charge batch action available to `MeetingManagers` when using
  `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup` or
  `MeetingConfig.includeGroupsInChargeDefinedOnCategory`.
  [gbastien]

#### Version 4.2.17 (2025-03-17)

- Make `test_pm_json_collections_count` more robust by disabling every workflow
  adaptations so a custom profile will not enable a `DashboardCollection`
  that is using a counter.
  [gbastien]
- In `MeetingItem.getGivenAdvices` use `toLocalizedTime`
  from `@@plone` instead python script.
  [gbastien]
- Do not close add/edit annex overlay when clicking outside of it.
  [gbastien]
- When duplicating an item and using groups in charge on the category, make sure
  the new item uses groups in charge defined on the category and not original
  item groups in charge in case configuration was changed on the category.
  Make also sure that when an item is sent to another `MeetingConfig`, groups
  in charge defined on destination category are correctly applied on new item.
  On the `MeetingItem` view, do not `includeAuto=True` for groups in charge,
  display really stored groups in charge.
  [gbastien]

#### Products.MeetingCommunes (4.2.11 → 4.2.12)

#### Version 4.2.12 (2025-03-24)

- Added possibility to get generated finance advice for restapi in
  new key `deliberation_finance_advice`.
  [gbastien]

#### imio.pm.locales (4.2.23 → 4.2.24)

#### Version 4.2.24 (2025-03-24)

- Added translation for `pt_mailing_will_be_sent_to`.
  [gbastien]

## Release 4.2.31.4

**Date:** 2025-03-12

### Package Updates

#### Products.PloneMeeting (4.2.15 → 4.2.16)

#### Version 4.2.16 (2025-03-11)

- Fixed `@@json_collections_count` caching invalidation for collections using
  a criterion refering to current connected user.
  [gbastien]
- Added new advice type `Positive after modification`.
  [gbastien]
- Added `fplog` when inserting/removing item from meeting.
  [gbastien]
- When not using the `decided` meeting workflow state,
  meeting is always considered `decided`.
  [gbastien]
- Optimized `MeetingItem.getMeetingToInsertIntoWhenNoCurrentMeetingObject`
  cachekey to not cache per item but per `MeetingConfig` and only consider
  `preferredMeeting`.
  [gbastien]
- On item templates and recurring items make sure every active delay aware
  advisers are displayed, ignore the `for_item_created_from` information.
  [gbastien]
- Fixed POD template mailing list containing a quote (') was breaking JS.
  [gbastien]
- Added logging when reindexing every items icon color
  when changed in `MeetingConfig`.
  [gbastien]

#### Products.MeetingCommunes (4.2.10 → 4.2.11)

#### Version 4.2.11 (2025-03-11)

- Adapted `zcity` profile to use `contactsTemplates` from `examples_fr` profile.
  [gbastien]

#### collective.contact.core (1.39 → 1.43.1)

#### Version 1.43.1 (2025-02-28)

- Added libjpeg8 for Pillow install in gha.
  [sgeulette]
- Added libbz2-dev for feedparser install in gha.
  [sgeulette]
- Moved include package `imio.fpaudit` from `testing.zcml` to `configure.zcml`.
  [gbastien]

#### Version 1.43.0 (2025-02-20)

- Added audit_access function, called at some places, to log contact access.
  [sgeulette]

#### Version 1.42.0 (2023-09-13)

- Set mail index lowercase.
  [sgeulette]

#### Version 1.41 (2023-09-07)

- Improved date ranges.
  [sgeulette]

#### Version 1.40 (2023-07-20)

- Added plone.app.iterate dependency.
  [sgeulette]
- Replaced subscribers grok declaration by zcml
  [sgeulette]
- Added subscribers docstrings
  [sgeulette]
- fix: [DMS-949] min & max for start_date, end_date
  [bleybaert]

#### collective.documentgenerator (3.43 → 3.44)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.16.1 → 1.16.2)

#### Version 1.16.2 (2025-02-28)

- Overrided `Form.__call__` to not render if request reponse status
  is 204 (No content) as it is already the case when response status is 302 or
  the portal message is not displayed after faceted refresh because
  it was already displayed on the closing form.
  [gbastien]
- Added Attributes in modified call to specify which attribute has been modified.
  [cadam, sgeulette]
- Corrected typo
  [sgeulette]

#### imio.pm.locales (4.2.22 → 4.2.23)

#### Version 4.2.23 (2025-03-11)

- Added translations for `Change committees` batch action.
  [gbastien]
- Added translations for new advice type `Positive after modification`.
  [gbastien]

#### plonetheme.imioapps (2.50 → 2.51)

#### Version 2.51 (2025-03-11)

- If current URL contains `imio-acceptation`,
  highlight `portal-header` (turn it red).
  [gbastien]

## Release 4.2.31.3

**Date:** 2025-02-06

### Package Updates

#### Products.PloneMeeting (4.2.14 → 4.2.15)

#### Version 4.2.15 (2025-02-06)

- Optimized `Meeting._update_using_groups_local_roles` that may be called on
  every existing meetings when saving several organizations in parameter
  `MeetingConfig.usingGroups`.
  This leaded to several minutes to save the `MeetingConfig`.
  [gbastien]
- Added confirmation dialog when clicking on `Send to other MeetingConfig`
  button as this will send the item to another `MeetingConfig` immediately.
  [gbastien]
- For `Delete whole meeting` confirm dialog message,
  use specific message `plonemeeting_delete_meeting_confirm_message`.
  [gbastien]
- In `PloneGroupSettingsOrganizationsValidator` display full `MeetingConfig`
  title (including `configGroup` label) in case several `MeetingConfigs` with
  same title exist in different config groups.
  [gbastien]

#### imio.helpers (1.0.0rc3 → 1.2.2)

#### Version 1.2.2 (2025-02-06)

- Added parameters `ask_confirm=false, confirm_msg='are_you_sure'` to
  JS function `callViewAndReload` so it is possible to have a
  confirmation dialog to execute the action or not.
  [gbastien]

#### Version 1.2.1 (2025-01-20)

- Improved `emailer.send_email` to take into account 3.10.12 python bug.
  [sgeulette]
- Removed ipython
  [sgeulette]

#### Version 1.2.0 (2024-12-19)

- Added new parameter to `batching.batch_get_keys`.
  [sgeulette]

#### Version 1.1.0 (2024-10-02)

- Imported batch_delete_files from imio.pyutils if someone is yet using it from here.
  [sgeulette]
- batch is considered finished if no batching.
  [sgeulette]

#### Version 1.0.1 (2024-09-18)

- Generated universal wheel version.
  [sgeulette]

#### Version 1.0.0rc4 (2024-07-08)

- Added "empty" variables to handle empty indexes searches.
  [sgeulette]

#### collective.contact.plonegroup (1.51 → 1.52)

#### Version 1.52 (2025-02-06)

- Added parameter `verify_group_exist=True` to `utils.get_plone_groups`.
  When set to `False`, it will not get the real Plone group object to check
  if it exist when using `ids_only=True`. In this case it is much faster.
  [gbastien]

## Release 4.2.31.2

**Date:** 2025-02-04

### Package Updates

#### Products.PloneMeeting (4.2.13 → 4.2.14)

#### Version 4.2.14 (2025-02-03)

- Fixed an issue when `MeetingItem.proposingGroupWithGroupInCharge` is used in a
  `MeetingConfig` but not in another one when an item is sent to it.
  [aduchene]
- Prevent to unselect an organization in plonegroup that
  is used by `MeetingConfig.usingGroups`.
  [gbastien]
- Fixed `otherMeetingConfigsClonableToFieldXXX` field management when it is
  empty, it was not emptying the value on new item, now it is the case except
  for `title` that can not be empty.
  [gbastien]
- Make `MeetingItem.marginalNotes` field editable by `MeetingManagers` when item
  is `presented` (before it was when item was `itemfrozen`) so votes are also
  editable when item is `presented` as it relies on same permission
  `WriteMarginalNotes` that we should change name to a more generic name like
  `WriteClosedMeetingMeetingManagersReservedFields`.
  [gbastien]
- Renamed `_get_default_attendees` to `get_default_attendees`,
  `_get_default_signatories` to `get_default_signatories` and
  `_get_default_voters` to `_get_default_voters` and added it to `safe_utils`
  so it may be used in restricted python code.
  [gbastien]
- Added parameter `signatories={}` to `BaseDGHV.print_signatories_by_position`
  to be able to pass a dict of arbitrary held positions to render as signatures.
  This is useful for printing default signatories for example when we do
  not want to use signatories defined on context (item or meeting).
  [gbastien]
- Fixed `PMAttendeeRedefinePositionTypesVocabulary` that did not render default
  value term of `IRedefineAttendeePosition.position_type` correctly when it was
  not in the base vocabulary.
  [gbastien]
- Display `MeetingConfig` title in page title (displayed in web browser tab)
  on faceted contexts (dashboard and in configuration) so user knows where he is
  when using several tabs.
  [gbastien]
- Fixed `PMCategorizedObjectAdapter.can_view` when managing not viewable items
  because it could lead to unwanted users having access to some annexes by
  accessing it's URL directly.
  [gbastien]
- Make sure annexes only previewable (not downloadable) are not selectable
  when duplicating an item, exporting it to PDF or exporting annexes to Zip.
  [gbastien]
- Renamed `Migrator.updateItemFilters` to `Migrator.update_faceted_filters` and
  `Migrator.cleanUsedItemAttributes` to `Migrator.update_used_attrs` and
  manage `to_add/to_remove/to_replace` for each methods.
  [gbastien]
- In the votes editing form, highlight the value selected by the radio button
  as in some application the radio button is before or after the value.
  Renamed forms `item_encode_votes_form` to `item-encode-votes-form` and
  `item_encode_secret_votes_form` to `item-encode-secret-votes-form`.
  [gbastien]
- Prevent closing overlays when clicking outside it if it contains a form
  so we avoid losing encoded data if user clicked outside by mistake.
  [gbastien]
- Make `return_to_proposing_group` with validations more standalone by
  generating everything based on the `MeetingConfig.itemWFValidationLevels`.
  [gbastien]

#### imio.actionspanel (1.68 → 1.69)

#### Version 1.69 (2025-02-03)

- Prevent closing the workflow transition comment overlay when clicking outside
  it so we avoid losing comment in case user click outside by mistake.
  [gbastien]

#### imio.annex (2.23 → 2.24)

#### Version 2.24 (2025-02-03)

- Fixed `DownloadAnnexesBatchActionForm` to not download annexes that are only
  previewable (annexes for which `show_download` is `False`).
  [gbastien]

#### imio.pyutils (1.0.3 → 1.1.2)

#### Version 1.1.2 (2024-12-19)

- Improved `batching.batch_delete_files`.
  [sgeulette]

#### Version 1.1.1 (2024-09-18)

- Generated universal wheel version.
  [sgeulette]

#### Version 1.1.0 (2024-09-17)

- Added `utils.add_key_if_value` to add a key in a dic only if value or is not None.
  [sgeulette]
- Moved `batching.batch_delete_files` from imio.helpers to be used commonly.
  [sgeulette]

#### Version 1.0.4 (2024-06-11)

- Blacked files.
  [sgeulette]
- Added `system.post_request` to send a POST request.
  [sgeulette]

#### collective.eeafaceted.batchactions (1.15 → 1.16.1)

#### Version 1.16.1 (2025-02-03)

- Check again `self.do_apply` in `BaseBatchActionForm.handleApply` to avoid
  nasty behaviors.
  [gbastien]

#### Version 1.16.0 (2024-12-19)

- Overrided `ContactBaseBatchActionForm.available` method to handle anonymous
  search correctly.
  [sgeulette]

#### collective.iconifiedcategory (0.67 → 0.68)

#### Version 0.68 (2025-02-03)

- Fixed `CategorizedObjectAdapter.can_view` default implementation that was
  checking `View` permission on context but we need to check on
  `categorized_obj` as permissions could be different.
  [gbastien]

#### imio.pm.locales (4.2.21 → 4.2.22)

#### Version 4.2.22 (2025-02-03)

- Added translations for `can_not_unselect_plone_group_meetingconfig`.
  [gbastien]
- Added translations related to only previewable annexes not duplicated.
  [gbastien]
- Adapted `return_to_proposing_group` with validation WFA related translations.
  Removed no more used `returned_to_proposing_group_with_validation_state`.
  [gbastien]
- Overrided `collective.iconifiedcategory` translation of
  `Show preview description.` to be more specific regarding `PloneMeeting`.
  [gbastien]

## Release 4.2.31.1

**Date:** 2024-12-06

### Package Updates

#### Products.PloneMeeting (4.2.12 → 4.2.13)

#### Version 4.2.13 (2024-12-06)

- Fixed `MeetingConfig.itemsNotViewableVisibleFields` functionnality that was
  raising `Unhautorized` when accessing more infos of not viewable items.
  [gbastien]

## Release 4.2.31

**Date:** 2024-11-14

### Package Updates

#### Products.PloneMeeting (4.2.12rc1 → 4.2.12)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.9 → 4.2.10)

#### Version 4.2.10 (2024-11-07)

- Adapted `zcity` profile so `annexeDecisionToSign` and `annexeDecisionSigned`
  annex types are already configured by default.
  [gbastien]

#### imio.pm.locales (4.2.20.2 → 4.2.21)

#### Version 4.2.21 (2024-11-07)

- Removed unused translation `restricted_copy_groups_item_descr`.
  [gbastien]
- Added translations for `PloneMeeting_label_emergencyMotivation`.
  [gbastien]

## Release 4.2.30-test3

**Date:** 2024-10-17

### Package Updates

#### Products.PloneMeeting (4.2.11.2 → 4.2.12rc1)

#### Version 4.2.12 (2024-11-07)

- Added possibility to pass any parameter to `held_position.get_short_title`
  when using `BaseDGHV.print_attendees` and `BaseDGHV.print_attendees_by_type`
  using a special parameter `short_title_kwargs`.
  [gbastien]
- Added holidays for 2025.
  [aduchene]
- Completed `AnnexTypeDescriptors` and `ToolInitializer` to manage
  attribute `after_scan_change_annex_type_to`.
  Completed init attributes of `AnnexSubTypeDescriptor` and
  `ItemAnnexSubTypeDescriptor`.
  [gbastien]

## Release 4.2.30-test2

**Date:** 2024-10-16

### Package Updates

#### Products.PloneMeeting (4.2.11.1 → 4.2.11.2)

*No changelog entries found.*

#### imio.pm.locales (4.2.20.1 → 4.2.20.2)

*No changelog entries found.*

#### plonemeeting.restapi (2.7 → 2.8)

#### Version 2.8 (2024-10-16)

- Adapted call to `get_attendee_short_title` as it was moved
  from `Meeting` to `utils`.
  [gbastien]

## Release 4.2.30-test

**Date:** 2024-10-02

### Package Updates

#### Products.PloneMeeting (4.2.11 → 4.2.11.1)

*No changelog entries found.*

#### collective.contact.plonegroup (1.50 → 1.51)

#### Version 1.51 (2024-10-02)

- Added helpers `utils.enable_function` and `utils.disable_function`
  to easily enable/disable a function.
  [gbastien]

#### imio.pm.locales (4.2.20 → 4.2.20.1)

*No changelog entries found.*

## Release 4.2.29

**Date:** 2024-09-25

### Package Updates

#### Products.PloneMeeting (4.2.10 → 4.2.11)

#### Version 4.2.11 (2024-09-25)

- Added new field `MeetingItem.emergencyMotivation` to manage emergency
  motivation more easily and out of full `emergency` functionnality.
  Added monkeypatch to initialize a new HTML field correctly on existing elements.
  [gbastien]
- Upgrade `appy.pod` ready for `LibreOffice 24.2.x`.
  [gbastien]
- Let role `Manager` be able to remove an inherited advice in any case.
  [gbastien]

#### Products.MeetingCommunes (4.2.8 → 4.2.9)

#### Version 4.2.9 (2024-09-25)

- Fixed typo in finances advice sentences (`prealable > préalable`).
  [gbastien]

#### appy (1.0.15 → 1.0.18)

*No changelog entries found.*

#### imio.annex (2.22 → 2.23)

#### Version 2.23 (2024-09-25)

- Fixed XSS vulnerability in annexes table `PrettyLinkColumn`.
  [gbastien]

#### imio.history (1.35 → 1.36)

#### Version 1.36 (2024-09-25)

- Added `utils.get_all_history_attr` to `safe_utils`.
  [gbastien]

#### imio.pm.locales (4.2.19 → 4.2.20)

#### Version 4.2.20 (2024-09-25)

- Fixed typo in french translation of `PloneMeeting_label_itemPreferredMeetingStates`.
  [gbastien]
- Added translation for new `MeetingItem.emergencyMotivation` field.
  [gbastien]

#### plonetheme.imioapps (2.49 → 2.50)

#### Version 2.50 (2024-09-25)

- Fixed faceted dashboard header height to avoid 1px blank space between
  global header and dashboard table header when scrolling
  (sticky dashboard table header).
  [gbastien]

## Release 4.2.28

**Date:** 2024-09-19

### Package Updates

#### Products.PloneMeeting (4.2.9.1 → 4.2.10)

#### Version 4.2.10 (2024-09-19)

- Display a clear message when trying to remove a meeting containing items as
  `MeetignManager` as it will raise `Unauthorized` when using restapi.
  [gbastien]
- Fixed `PMPortalTypesVocabulary` to use portal_type `Title` method to display
  the term title instead translating the term `title` attribute.
  [gbastien]
- Adapted `adaptations.RETURN_TO_PROPOSING_GROUP_MAPPINGS` to be able to define
  the list of meeting states on a per `MeetingConfig` basis.
  [gbastien]
- Fixed `AskedAdvicesVocabulary` to mark an term as inactive only if
  `for_item_created_until` date is actually expired.
  [gbastien]
- Fix issue regarding mail notification not sent when user is coming from a LDAP/AD.
  [aduchene]
- Adapted `MeetingItem.restrictedCopyGroups` so it is only editable by
  `MeetingManager`.
  [gbastien]

#### Version 4.2.9rc6 (2024-04-10)

- Moved field `Meeting.pre_observations` before `Meeting.observations`.
  [gbastien]
- Make `test_pm_WFA_availableWFAdaptations` more robust by generating the
  `presented_item_back_to_` WF adaptations as it relies on defined
  `MeetingConfig.itemWFValidationLevels`.
  [gbastien]
- Make tests using `utils.set_field_from_ajax` more robust by using field
  `description` instead `decision` as in some case (subplugin), `decision`
  field is not writable.
  [gbastien]
- Do not automatically reinitialize the delay of an advice during the
  `MeetingConfig.transitionsReinitializingDelays` if delay was timed out,
  this will have to be done manually.
  [gbastien]
- Renamed `test_pm_WFA_waiting_advices` to `test_pm_WFA_waiting_advices_base`
  so it can be executed separately than other `test_pm_WFA_waiting_advices_`
  tests.
  Completed `test_pm_ItemActionsPanelCachingProfiles` to check when reviewer
  may also edit crated item (when using `extra_suffixes`), this way we may
  remove `_reviewers_may_edit_itemcreated` helper.
  [gbastien]
- Fixed `test_pm_ItemMailNotificationLateItem` when called from subplugins.
  [gbastien]
- Make `test_pm_Validate_itemWFValidationLevels_removed_depending_used_state_item`
  and `test_pm_SearchItemsToCorrectToValidateOfEveryReviewerGroups` more robust
  when called from subplugin.
  [gbastien]
- Adapted `Products.PloneMeeting.vocabularies.advicetypesvocabulary`, used in
  advice types faceted filter to take into account
  `ToolPloneMeeting.advisersConfig.advice_types`.
  [gbastien]
- Add two types of email notifications to suffixes about given advices.
  Added upgrade step to 4214 to update `MeetingConfig.mailItemEvents`.
  [aduchene]
- Add a notification to power observers about late items.
  [aduchene]
- When `MeetingConfig.mailMode` is set to `test`, display the sent mail `subject`
  and `recipients` in a portal message.
  [gbastien]
- Do not break in `MeetingConfig` POD templates when some reusable POD templates
  were deleted or marked no more reusable.
  [gbastien]
- Import `safe_encode` from `imio.pyutils` instead `imio.helpers`.
  [gbastien]
- Now that `@@folder_contents` works on `DashboardCollection`,
  added `test_pm_Folder_contents` to confirm it.
  [gbastien]
- Added `tobytes` and `fileSize` from `Products.CPUtils` to `safe_utils`, this
  is necessary to convert `portal_catalog` `getObjSize` format to `bytes` and
  `bytes` to a human readable format.
  [gbastien]
- Back to previous behavior in `utils._sendMail`, when sending an email
  with attachment, send it only one time to every recipients instead sending
  it one time by recipient.
  [gbastien]
- Avoid vocabulary `AskedAdvicesVocabulary` being empty when cached because
  `MeetingConfig` could not be obtained.
  [gbastien]
- Display `MeetingConfig.usingGroups` field on `MeetingConfig` view home page
  under `Groups and users` to identify easily a MeetingConfig using this parameter.
  [gbastien]
- Added parameters `withItemNumber=False` and `withItemReference=False` to
  `MeetingItem.Title` to have the item title prefixed with item reference
  and/or item number.
  [gbastien]
- Adapted `utils._sendMail` to use `bcc` (`blind carbon copy`) when sending
  an email with attachment (one email sent to several recipients).
  [gbastien]
- Display `TAL condition` by default on `MeetingConfig` view in
  `POD templates` section.
  [gbastien]

#### Version 4.2.9rc5 (2024-03-14)

- Added upgrade step to 4213 to fix POD templates that were using
  `.adapted().getCertifiedSignatures()` to `.getCertifiedSignatures()`,
  `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]

#### Version 4.2.9rc4 (2024-03-14)

- Added `org_uid` to elements available when evaluating the TAL expression on an
  organization to compute `as_copy_groups_on`.
  [gbastien]
- Adapted `MeetingCategory.is_selectable`, will no more be selectable if
  functionnality not enabled in `MeetingConfig`.
  [gbastien]
- Added warning on MeetingConfig view in the POD templates section to warn user
  to edit templates only if relevant and to never user MS Word.
  [gbastien]
- Avoid `UnicodeDecodeError` in `ConfigHideHistoryTosVocabulary`.
  [gbastien]
- `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]
- Moved field `advice.advice_reference` under `advice.advice_accounting_commitment`
  so `RichText` fields are grouped together.
  Display `advice_reference` in advice tooltipster when not empty.
  [gbastien]

#### Version 4.2.9rc3 (2024-03-05)

- Fixed custom advice WF UI:

  - do not display `given_by` information when using the default advice workflow;
  - in `onAdviceTransition` event, notify `AdviceAfterTransitionEvent` after
    `hidden_during_redaction` auto set to `False` management;
  - adapted import_data to manage `advisersConfig`.

  [gbastien]
- Display advice type id when using vocabulary `ConfigAdviceTypes` in the configuration.
  [gbastien]
- Removed redirect from `ChangeItemCompletenessView._changeCompleteness`, this
  is already managed in the `__call__` method, this avoid a redirect when calling
  `_changeCompleteness` directly from another code, like an event.
  [gbastien]
- Added some padding top of custom advice message on advice view.
  [gbastien]
- Optimized `MeetingItem._updateAdvices` to avoid several computation of
  advisers when using inherited advices. This also fixes problem with optional
  key that was wrongly initialized for inherited advices.
  [gbastien]
- Removed unused vocabularies `PMEveryCategoryVocabulary` and
  `PMEveryCategoryTitleVocabulary`.
  [gbastien]

#### Version 4.2.9rc2 (2024-02-26)

- Added helper `MeetingConfig.get_transitions_to_close_a_meeting`.
  Removed adaptable method `MeetingItemWorkflowActions._latePresentedItemTransitions`
  no more necessary as this is managed automatically now based on
  `MeetingConfig.onMeetingTransitionItemActionToExecute`.
  [gbastien]
- Added `imio.helpers.date.formatDate` to `safe_utils` so it is available in
  TAL expressions.
  [gbastien]
- Make sure `print_votes` always return a string when `render_as_html=True`.
  [gbastien]
- Removed field `IPMPerson.userid`, instead use behavior
  `collective.contact.plonegroup.behaviors.IPlonegroupUserLink` that will add
  fields `userid` and `primary_organization`.  We use `primary_organization` as
  a way to manage default `proposingGroup` when creating an item.
  [gbastien]
- Fixed `utils._sendMail` to avoid `UnicodeDecodeError`.
  Also refactored it so the loop on recipients is managed by `utils._sendMail`
  and one mail is sent by recipient in any case (attachments or not).
  [gbastien]
- Use ZLogHandler in `ToolPloneMeeting.update_all_local_roles`.
  [aduchene]

#### Version 4.2.9b9 (2024-01-31)

- Make the advice `given_on` date use final WF state when using a custom WF.
  [gbastien]

#### Version 4.2.9b8 (2024-01-18)

- Do not `show_advice_on_final_wf_transition` when item is set in a wf state
  in which advice can not be edited anymore if advice did not reached it's final
  state (when using advice custom worklow).
  [gbastien]

#### Version 4.2.9b7 (2024-01-11)

- Added `Export PDF` action to `MeetingConfig.itemActionsColumnConfig`.
  [gbastien]

#### Version 4.2.9b6 (2024-01-11)

- Removed constant `config.ADVICE_STATES_ALIVE`, it is now managed automatically
  by `utils.get_advice_alive_states` and it will ne more be necessary to
  override it in custom profiles.
  [gbastien]
- In tests, use `imio.helpers.content.richtextval` everywhere a `RichTextValue` is used.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]

#### Version 4.2.9b5 (2024-01-02)

- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `Export PDF` action on item to be able to export in a single PDF file
  several selected PDF generated POD templates and PDF annexes.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Fixed CSS of advice popup label when very long.
  [gbastien]
- When `copyGroups` have access to item, highlight full `Copy groups` label in green.
  [gbastien]

#### Version 4.2.9b4 (2023-12-11)

- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]

#### Version 4.2.9b3 (2023-11-27)

- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]

#### Version 4.2.9b2 (2023-11-27)

- Display last transition actor and comment in item mail notifications for mail events:

  - `lateItem`;
  - `itemUnpresented`;
  - `itemDelayed`;
  - `itemPostponedNextMeeting`;
  - `returnedToProposingGroup`;
  - `returnedToMeetingManagers`.

  Added new item mail event `itemPostponedNextMeetingOwner`
  (in addition to `itemPostponedNextMeeting`).
  [gbastien]
- Fixed `ItemOptionalAdvicesVocabulary` caching to take into account delay aware
  advisers in cachekey as it is computed and depends on context.
  Fixed also a bug when some `__userid__` selected values were no more in the
  vocabulary with other values still in the vocabulary.
  [gbastien]
- Added `MeetingConfig.show_copy_groups_search` that is used to protect
  copyGroups related searches.
  [gbastien]
- Fixed `PMCategorizedChildView.__call___`, if no categorized elements,
  do not return just [] but the parameter `show_nothing` value,
  as it is rendered differently if True or False.
  [gbastien]
- Make `MeetingItem.meetingDeadlineDate` displayable in dashboards as static info
  (always visible in the item `Title` column).
  [gbastien]
- Static info `Item reference` is now selectable in the
  `MeetingConfig.availableItemsListVisibleColumns` as item reference may now be
  set before item is inserted into a meeting.
  [gbastien]
- Added `static_labels` and `static_item_reference` to the selectable values for
  `MeetingConfig.itemsVisibleFields` and `MeetingConfig.itemsNotViewableVisibleFields`.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_keep_internal_number`
  that will keep the `MeetingItem.internal_number` when `postpone_next_meeting`
  an item as the new item is somewhat the same presented again in another meeting.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_transfer_annex_scan_id`
  that will keep the annexes with a `scan_id` but transfer this `scan_id` from
  original annexes (where `scan_id` is set to None) to new annexes.
  [gbastien]
- Added `advice_hide_during_redaction_history` to store
  `advice.advice_hide_during_redaction` changes by user.
  [gbastien]
- Simplified `ToolPloneMeeting` to be able to move it to a registry adapter as
  light as possible, so remove most functionnalities from it:

  - Moved `ToolPloneMeeting.showMeetingView` to `MeetingFacetedView.show_page`
    as it is only used there;
  - Removed `TooPloneMeeting.getColoredLink`, use `MeetingItem.getPrettyLink`;
  - Moved `ToolPloneMeeting.getMailRecipient` to utils;
  - Moved `ToolPloneMeeting.getAdvicePortalTypes` and
    `ToolPloneMeeting.getAdvicePortalTypeIds` to utils;
  - Moved `ToolPloneMeeting.getAvailableMailingLists` to utils;
  - Removed no more used `versions_history_form.pt`;
  - Moved `ToolPloneMeeting.isPowerObserverForCfg` to
    `utils.isPowerObserverForCfg`;
  - Replaced `ToolPloneMeeting.getUserName` by
    `imio.helpers.content.get_user_fullname` everywhere it was used.

  [gbastien]
- Adapted `DisplayMeetingItemVoters` helper view on meeting to display items
  with `No vote` separately than items with `public` and `secret` votes and to
  not display it in non voted items anymore.
  [gbastien]
- Added faceted filter criterion `Item title only` to query items on
  items's title only using the `Title` index.
  [gbastien]
- When using `MeetingConfig.computeItemReferenceForItemsOutOfMeeting`, do not clear
  item reference when meeting back to `created` or when item back to `validated`.
  Renamed `MeetingItem.mustShowItemReference` to `MeetingItem.show_item_reference`.
  [gbastien]
- In dashboards displaying items, display `Proposing group` before `Category`
  and `Classifier`.
  [gbastien]
- Fixed update `categorized_elements` of advices when advice moved as
  stored path changed (when advice is given on an item that is `itemcreated` and
  that is renamed).
  [gbastien]
- Make sure every item related searches (Collection) use `sort_on` modified
  as this is not visible in the application because faceted `sort_on` overrides
  it but it is now taken into account when using restapi with a `base_search_uid`.
  [gbastien]

## Release 4.2.27.1

**Date:** 2024-10-28

### Package Updates

#### Products.PloneMeeting (4.2.9 → 4.2.9.1)

#### Version 4.2.9rc1 (2024-02-08)

- Adapted portal tabs sub menu styling to make more `sub menu`.
  [gbastien]
- Fixed critical bug while sending mail that was preventing to use the MailHost
  mail_queue because using `secureSend` from `Products.CMFPlone` that is
  deprecated and that use `immediate=True`.
  Now emails will be correctly using the mail_queue and start it when necessary.
  [gbastien]
- In `utils.updateAnnexesAccess`, make sure we do not acquire attribute
  `categorized_elements` or update is done several times, this is the case when
  called on an advice, the parent item attribute was used.
  [gbastien]
- Prevent a siteadmin from renaming an item linked to a meeting (an item that
  is no more in it's WF initial state) or it breaks the link with the meeting.
  [gbastien]

#### Version 4.2.9b1 (2023-10-27)

- Make the advice `given_on` date use final WF state when using a custom WF.
  [gbastien]


- Do not `show_advice_on_final_wf_transition` when item is set in a wf state
  in which advice can not be edited anymore if advice did not reached it's final
  state (when using advice custom worklow).
  [gbastien]


- Added `Export PDF` action to `MeetingConfig.itemActionsColumnConfig`.
  [gbastien]


- Removed constant `config.ADVICE_STATES_ALIVE`, it is now managed automatically
  by `utils.get_advice_alive_states` and it will ne more be necessary to
  override it in custom profiles.
  [gbastien]
- In tests, use `imio.helpers.content.richtextval` everywhere a `RichTextValue` is used.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]


- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `Export PDF` action on item to be able to export in a single PDF file
  several selected PDF generated POD templates and PDF annexes.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Fixed CSS of advice popup label when very long.
  [gbastien]
- When `copyGroups` have access to item, highlight full `Copy groups` label in green.
  [gbastien]


- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]


- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]


- Display last transition actor and comment in item mail notifications for mail events:

  - `lateItem`;
  - `itemUnpresented`;
  - `itemDelayed`;
  - `itemPostponedNextMeeting`;
  - `returnedToProposingGroup`;
  - `returnedToMeetingManagers`.

  Added new item mail event `itemPostponedNextMeetingOwner`
  (in addition to `itemPostponedNextMeeting`).
  [gbastien]
- Fixed `ItemOptionalAdvicesVocabulary` caching to take into account delay aware
  advisers in cachekey as it is computed and depends on context.
  Fixed also a bug when some `__userid__` selected values were no more in the
  vocabulary with other values still in the vocabulary.
  [gbastien]
- Added `MeetingConfig.show_copy_groups_search` that is used to protect
  copyGroups related searches.
  [gbastien]
- Fixed `PMCategorizedChildView.__call___`, if no categorized elements,
  do not return just [] but the parameter `show_nothing` value,
  as it is rendered differently if True or False.
  [gbastien]
- Make `MeetingItem.meetingDeadlineDate` displayable in dashboards as static info
  (always visible in the item `Title` column).
  [gbastien]
- Static info `Item reference` is now selectable in the
  `MeetingConfig.availableItemsListVisibleColumns` as item reference may now be
  set before item is inserted into a meeting.
  [gbastien]
- Added `static_labels` and `static_item_reference` to the selectable values for
  `MeetingConfig.itemsVisibleFields` and `MeetingConfig.itemsNotViewableVisibleFields`.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_keep_internal_number`
  that will keep the `MeetingItem.internal_number` when `postpone_next_meeting`
  an item as the new item is somewhat the same presented again in another meeting.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_transfer_annex_scan_id`
  that will keep the annexes with a `scan_id` but transfer this `scan_id` from
  original annexes (where `scan_id` is set to None) to new annexes.
  [gbastien]
- Added `advice_hide_during_redaction_history` to store
  `advice.advice_hide_during_redaction` changes by user.
  [gbastien]
- Simplified `ToolPloneMeeting` to be able to move it to a registry adapter as
  light as possible, so remove most functionnalities from it:

  - Moved `ToolPloneMeeting.showMeetingView` to `MeetingFacetedView.show_page`
    as it is only used there;
  - Removed `TooPloneMeeting.getColoredLink`, use `MeetingItem.getPrettyLink`;
  - Moved `ToolPloneMeeting.getMailRecipient` to utils;
  - Moved `ToolPloneMeeting.getAdvicePortalTypes` and
    `ToolPloneMeeting.getAdvicePortalTypeIds` to utils;
  - Moved `ToolPloneMeeting.getAvailableMailingLists` to utils;
  - Removed no more used `versions_history_form.pt`;
  - Moved `ToolPloneMeeting.isPowerObserverForCfg` to
    `utils.isPowerObserverForCfg`;
  - Replaced `ToolPloneMeeting.getUserName` by
    `imio.helpers.content.get_user_fullname` everywhere it was used.

  [gbastien]
- Adapted `DisplayMeetingItemVoters` helper view on meeting to display items
  with `No vote` separately than items with `public` and `secret` votes and to
  not display it in non voted items anymore.
  [gbastien]
- Added faceted filter criterion `Item title only` to query items on
  items's title only using the `Title` index.
  [gbastien]
- When using `MeetingConfig.computeItemReferenceForItemsOutOfMeeting`, do not clear
  item reference when meeting back to `created` or when item back to `validated`.
  Renamed `MeetingItem.mustShowItemReference` to `MeetingItem.show_item_reference`.
  [gbastien]
- In dashboards displaying items, display `Proposing group` before `Category`
  and `Classifier`.
  [gbastien]
- Fixed update `categorized_elements` of advices when advice moved as
  stored path changed (when advice is given on an item that is `itemcreated` and
  that is renamed).
  [gbastien]
- Make sure every item related searches (Collection) use `sort_on` modified
  as this is not visible in the application because faceted `sort_on` overrides
  it but it is now taken into account when using restapi with a `base_search_uid`.
  [gbastien]


- Added advanced advice management using `ToolPloneMeeting.advisersConfig`:

  - possible to associate a new advice `portal_type` to some organizations;
  - reworked advice infos template to add more CSS classes to additional infos;
  - display the `Advice given by` information;
  - added possibility to hide advice history to power observers and to everyone
    and to hide meeting history to powerobservers.

  [gbastien]
- Use `CompoundCriterion` adapter `living-items` for the `searchlivingitems`
  Collection so selected states are always correct if item workflow
  configuration changed.
  [gbastien]
- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]
- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]
- Display `created/modified` dates on `MeetingConfig view` for `categories`,
  `classifiers`, `recurring items`, `searches` and `pod templates`.
  [gbastien]
- Added in and out count to `print_attendees_by_type`.
  [aduchene]
- In `utils.set_field_from_ajax`, check again that user may actually edit given
  `field_name` to avoid malicious or erroneous use of it.
  [gbastien]
- Added new value `execute_tal_expression` for
  `MeetingConfig.onTransitionFieldTransforms.field_name`, this way it is now
  possible to define a TAL expression to execute after an item WF transition
  that will not change the content of a richtext field.
  [gbastien]

## Release 4.2.27-test

**Date:** 2024-07-19

### Package Updates

#### Products.PloneMeeting (4.2.9rc6 → 4.2.9)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.7 → 4.2.8)

#### Version 4.2.8 (2024-06-10)

- Fixed testing `import_data` configs title.
  [gbastien]
- Fixed demo profile that was not correctly tested because `MeetingConfig` id
  does not correspond in test.  Use `getId(True)` to get real mc id.
  [gbastien]
- Removed every MeetingConfig portal_types related translations as all this is generated now.
  [gbastien]

#### imio.actionspanel (1.64 → 1.68)

#### Version 1.68 (2024-06-07)

- Moved JS code to avoid double click on transition link to `imio.helpers`
  under name `temp_disable_link` and use it.
  [gbastien]
- Added back reverted code regarding `portal_type` title.
  [gbastien]

#### Version 1.67 (2024-05-27)

- Reverted change introduced in version 1.65 for now:
  Use `typeInfo.Title()` to get portal_type's title instead
  translating the `typeInfo.title`.
  [gbastien]

#### Version 1.66 (2024-05-27)

- Added `onObjWillBeRemoved` event handler (ZCML disabled by default)
  that will check for an `IContentDeletable.mayDelete` adapter upon
  any deletion.  Enable it when using `IContentDeletable`.
  [gbastien]

#### Version 1.65 (2024-02-08)

- Use `typeInfo.Title()` to get portal_type's title instead
  translating the `typeInfo.title`.
  [gbastien]

#### imio.helpers (1.0.0rc2 → 1.0.0rc3)

#### Version 1.0.0rc3 (2024-06-07)

- Added `temp_disable_link` JS helper that will disable a link for 2 seconds
  and to avoid double clicks.
  [gbastien]

#### imio.history (1.34 → 1.35)

#### Version 1.35 (2024-06-07)

- Moved translation of event comments to a sub method
  `IHContentHistoryView._translate_comments` so it is easier to override.
  [gbastien]

#### imio.pyutils (1.0.1 → 1.0.3)

#### Version 1.0.3 (2024-05-24)

- Fix bad release for python2.
  [aduchene]

#### Version 1.0.2 (2024-05-15)

- Added a new helper `utils.get_ordinal_clusters` to cluster ordinal numbers based on an offset.
  [aduchene]

#### imio.restapi (1.0rc1 → 1.0rc2)

*No changelog entries found.*

#### collective.behavior.internalnumber (0.3 → 0.4)

#### Version 0.4 (2024-06-07)

- Use `fti.Title()` that is a i18n `Message` instance to manage settings
  `portal_types` vocabulary.  Also sort vocabulary by term title.
  [gbastien]

#### collective.contact.plonegroup (1.49 → 1.50)

#### Version 1.50 (2024-05-27)

- Fixed `DisplayGroupUsersView.group_title` when `DisplayGroupUsersView.short=True`
  and group title contains several parenthesis.
  [gbastien]

#### collective.eeafaceted.z3ctable (2.26 → 2.27)

#### Version 2.27 (2024-05-27)

- When `the_object=True`, `attrName` may be a callable.
  [gbastien]

#### imio.pm.locales (4.2.17 → 4.2.19)

#### Version 4.2.19 (2024-06-10)

- Removed every portal_types related translations as this is generated now.
  [gbastien]

#### Version 4.2.18 (2024-05-27)

- Added translations related to `MeetingItem.restrictedCopyGroups`.
  [gbastien]
- Added translations related to `hide_decisions_when_under_writing__po__xxx`.
  [gbastien]

#### plonemeeting.restapi (2.5 → 2.7)

#### Version 2.7 (2024-06-07)

- Fixed french translation for `create_element_using_ws_rest`.
  [gbastien]

#### Version 2.6 (2024-05-27)

- Adapted `test_restapi_add_item_with_annexes_children` to show that annex
  `content_category` `only_pdf` parameter is taken into account.
  [gbastien]
- Added `testServiceDelete` to show that the `DELETE` method works as expected.
  [gbastien]
- Fixed french translation for `create_element_using_ws_rest_comments`.
  [gbastien]

#### plonetheme.imioapps (2.47 → 2.49)

#### Version 2.49 (2024-06-07)

- Use horizontal scroll when tooltipster is too large.
  [gbastien]

#### Version 2.48 (2024-05-27)

- Be more defensive when changing header color to red for test instances
  to avoid elements containing imio-test in id url being wrongly skinned.
  [gbastien]

## Release 4.2.26

**Date:** 2024-04-23

### Package Updates

#### Products.PloneMeeting (4.2.9rc6.post1 → 4.2.9rc6)

*No changelog entries found.*

## Release 4.2.26-wsc

**Date:** 2024-04-16

### Package Updates

#### Products.PloneMeeting (4.2.9rc5 → 4.2.9rc6.post1)

#### Version 4.2.9rc6 (2024-04-10)

- Moved field `Meeting.pre_observations` before `Meeting.observations`.
  [gbastien]
- Make `test_pm_WFA_availableWFAdaptations` more robust by generating the
  `presented_item_back_to_` WF adaptations as it relies on defined
  `MeetingConfig.itemWFValidationLevels`.
  [gbastien]
- Make tests using `utils.set_field_from_ajax` more robust by using field
  `description` instead `decision` as in some case (subplugin), `decision`
  field is not writable.
  [gbastien]
- Do not automatically reinitialize the delay of an advice during the
  `MeetingConfig.transitionsReinitializingDelays` if delay was timed out,
  this will have to be done manually.
  [gbastien]
- Renamed `test_pm_WFA_waiting_advices` to `test_pm_WFA_waiting_advices_base`
  so it can be executed separately than other `test_pm_WFA_waiting_advices_`
  tests.
  Completed `test_pm_ItemActionsPanelCachingProfiles` to check when reviewer
  may also edit crated item (when using `extra_suffixes`), this way we may
  remove `_reviewers_may_edit_itemcreated` helper.
  [gbastien]
- Fixed `test_pm_ItemMailNotificationLateItem` when called from subplugins.
  [gbastien]
- Make `test_pm_Validate_itemWFValidationLevels_removed_depending_used_state_item`
  and `test_pm_SearchItemsToCorrectToValidateOfEveryReviewerGroups` more robust
  when called from subplugin.
  [gbastien]
- Adapted `Products.PloneMeeting.vocabularies.advicetypesvocabulary`, used in
  advice types faceted filter to take into account
  `ToolPloneMeeting.advisersConfig.advice_types`.
  [gbastien]
- Add two types of email notifications to suffixes about given advices.
  Added upgrade step to 4214 to update `MeetingConfig.mailItemEvents`.
  [aduchene]
- Add a notification to power observers about late items.
  [aduchene]
- When `MeetingConfig.mailMode` is set to `test`, display the sent mail `subject`
  and `recipients` in a portal message.
  [gbastien]
- Do not break in `MeetingConfig` POD templates when some reusable POD templates
  were deleted or marked no more reusable.
  [gbastien]
- Import `safe_encode` from `imio.pyutils` instead `imio.helpers`.
  [gbastien]
- Now that `@@folder_contents` works on `DashboardCollection`,
  added `test_pm_Folder_contents` to confirm it.
  [gbastien]
- Added `tobytes` and `fileSize` from `Products.CPUtils` to `safe_utils`, this
  is necessary to convert `portal_catalog` `getObjSize` format to `bytes` and
  `bytes` to a human readable format.
  [gbastien]
- Back to previous behavior in `utils._sendMail`, when sending an email
  with attachment, send it only one time to every recipients instead sending
  it one time by recipient.
  [gbastien]
- Avoid vocabulary `AskedAdvicesVocabulary` being empty when cached because
  `MeetingConfig` could not be obtained.
  [gbastien]
- Display `MeetingConfig.usingGroups` field on `MeetingConfig` view home page
  under `Groups and users` to identify easily a MeetingConfig using this parameter.
  [gbastien]
- Added parameters `withItemNumber=False` and `withItemReference=False` to
  `MeetingItem.Title` to have the item title prefixed with item reference
  and/or item number.
  [gbastien]
- Adapted `utils._sendMail` to use `bcc` (`blind carbon copy`) when sending
  an email with attachment (one email sent to several recipients).
  [gbastien]
- Display `TAL condition` by default on `MeetingConfig` view in
  `POD templates` section.
  [gbastien]

#### Version 4.2.9b6 (2024-01-11)

- Removed constant `config.ADVICE_STATES_ALIVE`, it is now managed automatically
  by `utils.get_advice_alive_states` and it will ne more be necessary to
  override it in custom profiles.
  [gbastien]
- In tests, use `imio.helpers.content.richtextval` everywhere a `RichTextValue` is used.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]

#### imio.annex (2.21 → 2.22)

#### Version 2.22 (2024-04-10)

- Added parameter `filters={"to_print": True}` to `utils.get_annexes_to_print`
  so it is possible to filter annexes to print.
  [gbastien]
- Added concatenate annexes batch action to be able to produce a single PDF file
  from annex types of selected elements with two-sided management.
  Disabled by default (in `configure.zcml`).
  [gbastien]

#### imio.helpers (1.0.0rc1 → 1.0.0rc2)

#### Version 1.0.0rc2 (2024-04-10)

- Added batching module.
  [sgeulette]
- Fixed the way JS function `submitFormHelperOnsuccessDefault` manages
  returned result when it is a file, now we have a correct `filename`.
  [gbastien]
- Added transmogrifier Expression and Condition classes to log expression
  compilation or interpretation errors.
  [sgeulette]
- Removed `content.safe_encode` as already defined in `imio.pyutils`.
  Import it from `imio.pyutils` in `imio.helpers.content` for temporary backward
  compatibility, to be removed.
  [gbastien]
- Overrided `@@folder_contents` to make it work with `DashboardCollection`.
  [gbastien]
- Monkeypatched `plone.app.querystring.registryreader.getVocabularyValues`
  to keep vocabulary order onloy for Plone4, behavior is correct in Plone5+.
  Manage every `HAS_PLONE_X` values.
  [gbastien]

#### imio.history (1.33 → 1.34)

#### Version 1.34 (2024-04-10)

- Adapted `utils.getPreviousEvent` to add parameter `history_name='workflow'`.
  [gbastien]
- Fixed display of `HISTORY_COMMENT_NOT_VIEWABLE` in `@@contenthistory` view
  that was displayed as text, showing the HTML code.
  [gbastien]

#### imio.pyutils (1.0.0a1 → 1.0.1)

#### Version 1.0.1 (2024-04-08)

- Added patterns parameter in `system.read_dir_filter`.
  [sgeulette]
- Returned original filename in `system.hashed_filename` if string to hash is empty.
  [sgeulette]

#### collective.contact.plonegroup (1.48 → 1.49)

#### Version 1.49 (2024-04-10)

- Corrected behavior zcml definition to avoid message when Plone starts.
  [sgeulette]
- Import `safe_encode` from `imio.pyutils` instead `imio.helpers`.
  [gbastien]

#### collective.documentgenerator (3.39 → 3.43)

#### Version 3.43 (2024-04-10)

- Import `safe_encode` from `imio.pyutils` instead `imio.helpers`.
  [gbastien]
- Use has Plone versions constants (`HAS_PLONE_4`, `HAS_PLONE_5`, ...)
  from `imio.helpers`.
  [gbastien]

#### Version 3.42 (2024-02-12)

- Translated again type icon title.
  [gbastien]

#### Version 3.41 (2024-02-12)

- Corrected typo.
  [sgeulette]
- In `TitleColumn`, use `typeInfo.Title()` instead translating `typeInfo.title`,
  `Title()` do the same but manages special characters in the `title`.
  [gbastien]

#### Version 3.40 (2023-08-01)

- Add `DOCUMENTGENERATOR_LOG_PARAMETERS` environment variable that can be used to log request form parameters with
  collective.fingerpointing.
  [mpeeters]

#### collective.eeafaceted.batchactions (1.14 → 1.15)

#### Version 1.15 (2024-04-10)

- Import `safe_encode` from `imio.pyutils` instead `imio.helpers`.
  [gbastien]
- Check `available` in `update` instead in `handleApply` so form is not
  displayed at all if user have not access.
  [gbastien]

#### collective.eeafaceted.collectionwidget (1.16 → 1.17)

#### Version 1.17 (2024-04-10)

- Added `DashboardCollection.brains_results` that will return the result of the
  query as brains, this is used to make the `@@folder_contents` view work for
  `DashboardCollection` in `imio.helpers`.
  [gbastien]

#### collective.iconifiedcategory (0.64 → 0.67)

#### Version 0.67 (2024-04-10)

- Fixed utils.get_categorized_elements when `result_type='objects'`
  and `sort_on='getObjPositionInParent'`.
  [gbastien]
- Corrected typo in french translation of `Preview`.
  [gbastien]
- Removed optimization in `utils.validateFileIsPDF` to avoid multiple validation
  because it breaks validation of several elements added in the same `REQUEST`
  (when using rest api for example).
  [gbastien]
- Added `collective.iconifiedcategory.every_category_uids` vocabulary that
  lists every found categories with uid as vocabulary term token.
  [gbastien]

#### Version 0.66 (2024-02-27)

- Corrected bug due to typo.
  [sgeulette]

#### Version 0.65 (2024-02-19)

- Replaced container cloned event by moved event to handle rename,
  copy/paste and cut/paste of a container in the path.
  [sgeulette]
- Removed useless IconifiedModifiedEvent
  [sgeulette]
- Used `IIconifiedCategorizationMarker` in adequate subscribers definition
  [sgeulette]
- Removed some hasattr tests (MOD-831) and corrected events object
  [sgeulette]
- Handled cut/paste and rename of a categorized element
  [sgeulette]

#### imio.pm.locales (4.2.16 → 4.2.17)

#### Version 4.2.17 (2024-04-10)

- Added translations related to `advice_edited`, `advice_edited_in_meeting`
  and `late_item_in_meeting` item mail events.
  [gbastien]
- Added back wronlgy removed translations for `Duplicate and keep link`.
  [gbastien]

#### plonetheme.imioapps (2.45 → 2.47)

#### Version 2.47 (2024-04-10)

- URB-3007. Make caduc and abandoned workflow state grey in urban
  [jchandelle]
- Add justice contact icon
  [ndemonte]
- Added style for `concatenate-annexes` batch action button icon.
  [gbastien]
- Avoid `'NoneType' object has no attribute 'get'` in `ImioSearch.filter_query`
  if `query` is `None`.
  [gbastien]

#### Version 2.46 (2024-03-01)

- Added .apButtonAction_download background image.
  [sgeulette]

#### Products.CPUtils (1.23 → 1.25)

#### Version 1.25 (2024-04-10)

- Imported `safe_encode` from imio.pyutils.
  [sgeulette]

#### Version 1.24 (2024-02-12)

- Improved `set_attr`.
  [sgeulette]
- Added `obj_from_uid`
  [sgeulette]

## Release 4.2.25

**Date:** 2024-03-29

### Package Updates

#### Products.PloneMeeting (4.2.9rc2 → 4.2.9rc5)

#### Version 4.2.9rc5 (2024-03-14)

- Added upgrade step to 4213 to fix POD templates that were using
  `.adapted().getCertifiedSignatures()` to `.getCertifiedSignatures()`,
  `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]

#### Version 4.2.9rc4 (2024-03-14)

- Added `org_uid` to elements available when evaluating the TAL expression on an
  organization to compute `as_copy_groups_on`.
  [gbastien]
- Adapted `MeetingCategory.is_selectable`, will no more be selectable if
  functionnality not enabled in `MeetingConfig`.
  [gbastien]
- Added warning on MeetingConfig view in the POD templates section to warn user
  to edit templates only if relevant and to never user MS Word.
  [gbastien]
- Avoid `UnicodeDecodeError` in `ConfigHideHistoryTosVocabulary`.
  [gbastien]
- `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]
- Moved field `advice.advice_reference` under `advice.advice_accounting_commitment`
  so `RichText` fields are grouped together.
  Display `advice_reference` in advice tooltipster when not empty.
  [gbastien]

#### Version 4.2.9rc3 (2024-03-05)

- Fixed custom advice WF UI:

  - do not display `given_by` information when using the default advice workflow;
  - in `onAdviceTransition` event, notify `AdviceAfterTransitionEvent` after
    `hidden_during_redaction` auto set to `False` management;
  - adapted import_data to manage `advisersConfig`.

  [gbastien]
- Display advice type id when using vocabulary `ConfigAdviceTypes` in the configuration.
  [gbastien]
- Removed redirect from `ChangeItemCompletenessView._changeCompleteness`, this
  is already managed in the `__call__` method, this avoid a redirect when calling
  `_changeCompleteness` directly from another code, like an event.
  [gbastien]
- Added some padding top of custom advice message on advice view.
  [gbastien]
- Optimized `MeetingItem._updateAdvices` to avoid several computation of
  advisers when using inherited advices. This also fixes problem with optional
  key that was wrongly initialized for inherited advices.
  [gbastien]
- Removed unused vocabularies `PMEveryCategoryVocabulary` and
  `PMEveryCategoryTitleVocabulary`.
  [gbastien]

#### Version 4.2.9b5 (2024-01-02)

- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `Export PDF` action on item to be able to export in a single PDF file
  several selected PDF generated POD templates and PDF annexes.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Fixed CSS of advice popup label when very long.
  [gbastien]
- When `copyGroups` have access to item, highlight full `Copy groups` label in green.
  [gbastien]

#### Version 4.2.9b4 (2023-12-11)

- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]

#### Version 4.2.9b3 (2023-11-27)

- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]

#### Products.MeetingCommunes (4.2.6 → 4.2.7)

#### Version 4.2.7 (2024-03-14)

- Fix template_path not used for some templates in `example_fr` profile. 
  This prevented install from profiles located in other packages.
  [aduchene]
- Removed translations for advice WFA
  `meetingadvicefinances_controller_propose_to_manager` as it does not exist anymore.
  [gbastien]
- Fixed POD templates `deliberation.odt` and `deliberation_recto_verso.odt`,
  `MeetingItem.getCertifiedSignatures` is no more an adaptable method
  (removed `.adapted()`).
  [gbastien]

#### Version 4.2.6rc1 (2024-02-08)

- Added parameter `ignore_not_given_advice=False` to
  `CustomMeetingItem.showFinanceAdviceTemplate`, when `True`, this will hide
  the POD template when advice is `not_given` or `asked_again`.
  [gbastien]

#### Version 4.2.6b7 (2024-01-31)

- Added `test_pm_Show_advice_on_final_wf_transition_when_item_in_advice_not_giveable_state`
  that will test that when item is set to a state in which advice is no more
  editable, `advice.advice_hide_during_redaction` is not set back to `True`
  if advice was not in it's workflow final state (when using advice custom workflow).
  [gbastien]
- Adapted `test_Get_advice_given_by` to check that `get_advice_given_on` is
  the advice WF `signFinancialAdvice` transition date when using a custom WF.
  [gbastien]

#### Version 4.2.6b6 (2024-01-11)

- Adapted code to use `imio.helpers.content.richtextval` instead `RichTextValue` when possible.
  [gbastien]

#### Version 4.2.6b5 (2024-01-02)

- Added translations for the `add_advicecreated_state` WFA.
  [gbastien]
- Every item related search (Collection) use `sort_on` `modified` instead `created`.
  [gbastien]

#### Version 4.2.6b4 (2023-12-11)

- CSS, color in blue state `financial_advice_signed` in advice history.
  [gbastien]
- Adapted code as `ToolPloneMeeting.getUserName` is replaced by
  `imio.helpers.content.get_user_fullname` and
  `ToolPloneMeeting.isPowerObserverForCfg` is moved to
  `utils.isPowerObserverForCfg`.
  [gbastien]

#### Version 4.2.6b3 (2023-11-27)

- Added parameter `ignore_advice_hidden_during_redaction=False` to
  `CustomMeetingItem.showFinanceAdviceTemplate`, when `True`, this will hide
  the POD template when advice is hidden during redaction except if member is
  `MeetingManager` or in the advice `_advisers` group.
  [gbastien]

#### Version 4.2.6b2 (2023-11-27)

- Move back `add_advicecreated_state` advice WFA related code from `PloneMeeting`.
  [gbastien]
- Fixed `meetingadvicefinancs` `portal_type.allowed_content_types` install.
  [gbastien]
- Completed translations of finances advices types.
  [gbastien]

#### Version 4.2.6b1 (2023-10-27)

- Adapted code now that custom advice portal_types is managed by
  `ToolPloneMeeting.advisersConfig`:

  - Added new advice finances WF `meetingadvicefinancessimple_workflow`;
  - Fixed tests as `MeetingConfig.listWorkflowAdaptations` was removed.

  [gbastien]
- Added `Export users/groups` dashboard template for contacts in `examples_fr` profile.
  [gbastien]
- Updated `recapitulatif-tb.ods` to use `appy.pod` instruction `do cell from+ xhtml(...)`
  instead `view.display_html_as_text`.
  [gbastien]
- Fixed `CustomMeetingConfig.getUsedFinanceGroupIds` that was not working
  for auto asked advices.
  [gbastien]

#### imio.actionspanel (1.65 → 1.64)

*No changelog entries found.*

#### imio.restapi (1.0b3 → 1.0rc1)

*No changelog entries found.*

#### imio.pm.locales (4.2.15 → 4.2.16)

#### Version 4.2.16 (2024-03-14)

- Added translations for `warning_meetingconfig_edit_podtemplate_descr`.
  [gbastien]
- Added translations for `Advice accounting commitment` behavior.
  [gbastien]

#### plonemeeting.restapi (2.3 → 2.5)

#### Version 2.5 (2024-03-19)

- When using `fullobjects`, only serialize `next/previous` when specifically
  asked using `include_nextprev=true`.
  [gbastien]

#### Version 2.4 (2024-03-14)

- Fixed `test_restapi_add_clean_meeting`, when generating new date use datetime
  and timedelta to avoid generating an unexisting date,
  here it was generating `2025/02/29` that does not exist.
  [gbastien]
- When using `@users?extra_include=categories`, categories are only returned if
  enabled in `MeetingConfig`, same for `classifiers`, this avoid having
  selectable categories for an user when categories are not used.
  [gbastien]
- Added special behavior for `review_state` and `creators` when asked in
  `metadata_fields`:

  - `review_state` will return a token/title with review_state id
    and translated title;
  - `creators` will return a list of token/title with each creator id
    and fullname.

  [gbastien]

## Release 4.2.24

**Date:** 2024-02-26

### Package Updates

#### Products.PloneMeeting (4.2.8.2 → 4.2.9rc2)

#### Version 4.2.9 (2024-06-10)

- In `EveryAnnexTypesVocabulary` use `content_category` icon image scale
  instead `portal_url.getRelativeUrl` so it is cached.
  [gbastien]
- Execute `upgrade_step_4211_add_item_widgets.xml` adding faceted criterion
  `title only` again in upgrade to `4214` as it was not in
  `default_dashboard_items_widgets.xml`, new `MeetingConfig` added since
  profile version `4211` are missing this criterion.
  [gbastien]
- Completed `print_votes` so it manages every `vote_values`
  (`does_not_vote`, `not_found`, `invalid`, `blank`).
  Adapted parameter `single_vote_value` so we can define a single value or
  a different value for each `vote_values`.
  Adapted parameter `include_voters=False` that maye be False/True or a list of
  vote values.
  Added parameter `include_voters_percent_treshold=100` that is an integer value
  from 0 to 100 that will display voters if ratio between number of voters and
  total voters exceeds the treshold.
  [gbastien]
- Added field `MeetingItem.restrictedCopyGroups`, a secondary `copyGroups` field
  where we can define other groups having access to item in other (later) states.
  [gbastien]
- Now every deletion is protected by `IContentDeletable`, including default
  Plone deletion using `manage_delObjects`.
  [gbastien]
- Fixed item number not saved when using `Disk` icon to change item number
  on meeting view when item number is a subnumber.
  [gbastien]
- Fixed validation of meeting signatories when creating a meeting, it was possible
  to create a meeting with several signatories using same signature number.
  [gbastien]
- Added per power observer complementary workflow adaptation to base
  `hide_decisions_when_under_writing` to let the selected power observers
  have access to the item decision.
  [gbastien]
- Improve `view.print_attendees_by_type` to be able to customize the in and out
  count more.
  [aduchene]
- Allow to use OrderedDict in POD templates.
  [aduchene]
- Fixed attendees statistics wrong absent/excused computation in sheet by meeting.
  [gbastien]
- Integrate `imio.webspellchecker` to replace `Scayt` for `CKEditor`.
  As `WSC` is started when focus is set in `CKEditor` field, set focus on
  field when using quick edit.
  [gbastien]
- Avoid double click on POD template mailing list.
  [gbastien]
- Generate `Meeting/MeetingItem` portal_type title based on `MeetingConfig`
  title instead translating it.
  [gbastien]
- Optimized `@@load_item_assembly_and_signatures` especially when several
  voters (50) and votes for an item (25).
  [gbastien]
- Fixed encode votes for several items failed when there was a `no_vote` item
  in the way.
  [gbastien]

#### Version 4.2.9rc2 (2024-02-26)

- Moved field `Meeting.pre_observations` before `Meeting.observations`.
  [gbastien]
- Make `test_pm_WFA_availableWFAdaptations` more robust by generating the
  `presented_item_back_to_` WF adaptations as it relies on defined
  `MeetingConfig.itemWFValidationLevels`.
  [gbastien]
- Make tests using `utils.set_field_from_ajax` more robust by using field
  `description` instead `decision` as in some case (subplugin), `decision`
  field is not writable.
  [gbastien]
- Do not automatically reinitialize the delay of an advice during the
  `MeetingConfig.transitionsReinitializingDelays` if delay was timed out,
  this will have to be done manually.
  [gbastien]
- Renamed `test_pm_WFA_waiting_advices` to `test_pm_WFA_waiting_advices_base`
  so it can be executed separately than other `test_pm_WFA_waiting_advices_`
  tests.
  Completed `test_pm_ItemActionsPanelCachingProfiles` to check when reviewer
  may also edit crated item (when using `extra_suffixes`), this way we may
  remove `_reviewers_may_edit_itemcreated` helper.
  [gbastien]
- Fixed `test_pm_ItemMailNotificationLateItem` when called from subplugins.
  [gbastien]
- Make `test_pm_Validate_itemWFValidationLevels_removed_depending_used_state_item`
  and `test_pm_SearchItemsToCorrectToValidateOfEveryReviewerGroups` more robust
  when called from subplugin.
  [gbastien]
- Adapted `Products.PloneMeeting.vocabularies.advicetypesvocabulary`, used in
  advice types faceted filter to take into account
  `ToolPloneMeeting.advisersConfig.advice_types`.
  [gbastien]
- Add two types of email notifications to suffixes about given advices.
  Added upgrade step to 4214 to update `MeetingConfig.mailItemEvents`.
  [aduchene]
- Add a notification to power observers about late items.
  [aduchene]
- When `MeetingConfig.mailMode` is set to `test`, display the sent mail `subject`
  and `recipients` in a portal message.
  [gbastien]
- Do not break in `MeetingConfig` POD templates when some reusable POD templates
  were deleted or marked no more reusable.
  [gbastien]
- Import `safe_encode` from `imio.pyutils` instead `imio.helpers`.
  [gbastien]
- Now that `@@folder_contents` works on `DashboardCollection`,
  added `test_pm_Folder_contents` to confirm it.
  [gbastien]
- Added `tobytes` and `fileSize` from `Products.CPUtils` to `safe_utils`, this
  is necessary to convert `portal_catalog` `getObjSize` format to `bytes` and
  `bytes` to a human readable format.
  [gbastien]
- Back to previous behavior in `utils._sendMail`, when sending an email
  with attachment, send it only one time to every recipients instead sending
  it one time by recipient.
  [gbastien]
- Avoid vocabulary `AskedAdvicesVocabulary` being empty when cached because
  `MeetingConfig` could not be obtained.
  [gbastien]
- Display `MeetingConfig.usingGroups` field on `MeetingConfig` view home page
  under `Groups and users` to identify easily a MeetingConfig using this parameter.
  [gbastien]
- Added parameters `withItemNumber=False` and `withItemReference=False` to
  `MeetingItem.Title` to have the item title prefixed with item reference
  and/or item number.
  [gbastien]
- Adapted `utils._sendMail` to use `bcc` (`blind carbon copy`) when sending
  an email with attachment (one email sent to several recipients).
  [gbastien]
- Display `TAL condition` by default on `MeetingConfig` view in
  `POD templates` section.
  [gbastien]


- Added upgrade step to 4213 to fix POD templates that were using
  `.adapted().getCertifiedSignatures()` to `.getCertifiedSignatures()`,
  `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]


- Added `org_uid` to elements available when evaluating the TAL expression on an
  organization to compute `as_copy_groups_on`.
  [gbastien]
- Adapted `MeetingCategory.is_selectable`, will no more be selectable if
  functionnality not enabled in `MeetingConfig`.
  [gbastien]
- Added warning on MeetingConfig view in the POD templates section to warn user
  to edit templates only if relevant and to never user MS Word.
  [gbastien]
- Avoid `UnicodeDecodeError` in `ConfigHideHistoryTosVocabulary`.
  [gbastien]
- `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]
- Moved field `advice.advice_reference` under `advice.advice_accounting_commitment`
  so `RichText` fields are grouped together.
  Display `advice_reference` in advice tooltipster when not empty.
  [gbastien]


- Fixed custom advice WF UI:

  - do not display `given_by` information when using the default advice workflow;
  - in `onAdviceTransition` event, notify `AdviceAfterTransitionEvent` after
    `hidden_during_redaction` auto set to `False` management;
  - adapted import_data to manage `advisersConfig`.

  [gbastien]
- Display advice type id when using vocabulary `ConfigAdviceTypes` in the configuration.
  [gbastien]
- Removed redirect from `ChangeItemCompletenessView._changeCompleteness`, this
  is already managed in the `__call__` method, this avoid a redirect when calling
  `_changeCompleteness` directly from another code, like an event.
  [gbastien]
- Added some padding top of custom advice message on advice view.
  [gbastien]
- Optimized `MeetingItem._updateAdvices` to avoid several computation of
  advisers when using inherited advices. This also fixes problem with optional
  key that was wrongly initialized for inherited advices.
  [gbastien]
- Removed unused vocabularies `PMEveryCategoryVocabulary` and
  `PMEveryCategoryTitleVocabulary`.
  [gbastien]


- Added helper `MeetingConfig.get_transitions_to_close_a_meeting`.
  Removed adaptable method `MeetingItemWorkflowActions._latePresentedItemTransitions`
  no more necessary as this is managed automatically now based on
  `MeetingConfig.onMeetingTransitionItemActionToExecute`.
  [gbastien]
- Added `imio.helpers.date.formatDate` to `safe_utils` so it is available in
  TAL expressions.
  [gbastien]
- Make sure `print_votes` always return a string when `render_as_html=True`.
  [gbastien]
- Removed field `IPMPerson.userid`, instead use behavior
  `collective.contact.plonegroup.behaviors.IPlonegroupUserLink` that will add
  fields `userid` and `primary_organization`.  We use `primary_organization` as
  a way to manage default `proposingGroup` when creating an item.
  [gbastien]
- Fixed `utils._sendMail` to avoid `UnicodeDecodeError`.
  Also refactored it so the loop on recipients is managed by `utils._sendMail`
  and one mail is sent by recipient in any case (attachments or not).
  [gbastien]
- Use ZLogHandler in `ToolPloneMeeting.update_all_local_roles`.
  [aduchene]

#### Version 4.2.9rc1 (2024-02-08)

- Adapted portal tabs sub menu styling to make more `sub menu`.
  [gbastien]
- Fixed critical bug while sending mail that was preventing to use the MailHost
  mail_queue because using `secureSend` from `Products.CMFPlone` that is
  deprecated and that use `immediate=True`.
  Now emails will be correctly using the mail_queue and start it when necessary.
  [gbastien]
- In `utils.updateAnnexesAccess`, make sure we do not acquire attribute
  `categorized_elements` or update is done several times, this is the case when
  called on an advice, the parent item attribute was used.
  [gbastien]
- Prevent a siteadmin from renaming an item linked to a meeting (an item that
  is no more in it's WF initial state) or it breaks the link with the meeting.
  [gbastien]

#### Version 4.2.9b2 (2023-11-27)

- Make the advice `given_on` date use final WF state when using a custom WF.
  [gbastien]


- Do not `show_advice_on_final_wf_transition` when item is set in a wf state
  in which advice can not be edited anymore if advice did not reached it's final
  state (when using advice custom worklow).
  [gbastien]


- Added `Export PDF` action to `MeetingConfig.itemActionsColumnConfig`.
  [gbastien]


- Removed constant `config.ADVICE_STATES_ALIVE`, it is now managed automatically
  by `utils.get_advice_alive_states` and it will ne more be necessary to
  override it in custom profiles.
  [gbastien]
- In tests, use `imio.helpers.content.richtextval` everywhere a `RichTextValue` is used.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]


- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `Export PDF` action on item to be able to export in a single PDF file
  several selected PDF generated POD templates and PDF annexes.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Fixed CSS of advice popup label when very long.
  [gbastien]
- When `copyGroups` have access to item, highlight full `Copy groups` label in green.
  [gbastien]


- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]


- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]


- Display last transition actor and comment in item mail notifications for mail events:

  - `lateItem`;
  - `itemUnpresented`;
  - `itemDelayed`;
  - `itemPostponedNextMeeting`;
  - `returnedToProposingGroup`;
  - `returnedToMeetingManagers`.

  Added new item mail event `itemPostponedNextMeetingOwner`
  (in addition to `itemPostponedNextMeeting`).
  [gbastien]
- Fixed `ItemOptionalAdvicesVocabulary` caching to take into account delay aware
  advisers in cachekey as it is computed and depends on context.
  Fixed also a bug when some `__userid__` selected values were no more in the
  vocabulary with other values still in the vocabulary.
  [gbastien]
- Added `MeetingConfig.show_copy_groups_search` that is used to protect
  copyGroups related searches.
  [gbastien]
- Fixed `PMCategorizedChildView.__call___`, if no categorized elements,
  do not return just [] but the parameter `show_nothing` value,
  as it is rendered differently if True or False.
  [gbastien]
- Make `MeetingItem.meetingDeadlineDate` displayable in dashboards as static info
  (always visible in the item `Title` column).
  [gbastien]
- Static info `Item reference` is now selectable in the
  `MeetingConfig.availableItemsListVisibleColumns` as item reference may now be
  set before item is inserted into a meeting.
  [gbastien]
- Added `static_labels` and `static_item_reference` to the selectable values for
  `MeetingConfig.itemsVisibleFields` and `MeetingConfig.itemsNotViewableVisibleFields`.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_keep_internal_number`
  that will keep the `MeetingItem.internal_number` when `postpone_next_meeting`
  an item as the new item is somewhat the same presented again in another meeting.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_transfer_annex_scan_id`
  that will keep the annexes with a `scan_id` but transfer this `scan_id` from
  original annexes (where `scan_id` is set to None) to new annexes.
  [gbastien]
- Added `advice_hide_during_redaction_history` to store
  `advice.advice_hide_during_redaction` changes by user.
  [gbastien]
- Simplified `ToolPloneMeeting` to be able to move it to a registry adapter as
  light as possible, so remove most functionnalities from it:

  - Moved `ToolPloneMeeting.showMeetingView` to `MeetingFacetedView.show_page`
    as it is only used there;
  - Removed `TooPloneMeeting.getColoredLink`, use `MeetingItem.getPrettyLink`;
  - Moved `ToolPloneMeeting.getMailRecipient` to utils;
  - Moved `ToolPloneMeeting.getAdvicePortalTypes` and
    `ToolPloneMeeting.getAdvicePortalTypeIds` to utils;
  - Moved `ToolPloneMeeting.getAvailableMailingLists` to utils;
  - Removed no more used `versions_history_form.pt`;
  - Moved `ToolPloneMeeting.isPowerObserverForCfg` to
    `utils.isPowerObserverForCfg`;
  - Replaced `ToolPloneMeeting.getUserName` by
    `imio.helpers.content.get_user_fullname` everywhere it was used.

  [gbastien]
- Adapted `DisplayMeetingItemVoters` helper view on meeting to display items
  with `No vote` separately than items with `public` and `secret` votes and to
  not display it in non voted items anymore.
  [gbastien]
- Added faceted filter criterion `Item title only` to query items on
  items's title only using the `Title` index.
  [gbastien]
- When using `MeetingConfig.computeItemReferenceForItemsOutOfMeeting`, do not clear
  item reference when meeting back to `created` or when item back to `validated`.
  Renamed `MeetingItem.mustShowItemReference` to `MeetingItem.show_item_reference`.
  [gbastien]
- In dashboards displaying items, display `Proposing group` before `Category`
  and `Classifier`.
  [gbastien]
- Fixed update `categorized_elements` of advices when advice moved as
  stored path changed (when advice is given on an item that is `itemcreated` and
  that is renamed).
  [gbastien]
- Make sure every item related searches (Collection) use `sort_on` modified
  as this is not visible in the application because faceted `sort_on` overrides
  it but it is now taken into account when using restapi with a `base_search_uid`.
  [gbastien]

#### Version 4.2.9b1 (2023-10-27)

- Added advanced advice management using `ToolPloneMeeting.advisersConfig`:

  - possible to associate a new advice `portal_type` to some organizations;
  - reworked advice infos template to add more CSS classes to additional infos;
  - display the `Advice given by` information;
  - added possibility to hide advice history to power observers and to everyone
    and to hide meeting history to powerobservers.

  [gbastien]
- Use `CompoundCriterion` adapter `living-items` for the `searchlivingitems`
  Collection so selected states are always correct if item workflow
  configuration changed.
  [gbastien]
- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]
- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]
- Display `created/modified` dates on `MeetingConfig view` for `categories`,
  `classifiers`, `recurring items`, `searches` and `pod templates`.
  [gbastien]
- Added in and out count to `print_attendees_by_type`.
  [aduchene]
- In `utils.set_field_from_ajax`, check again that user may actually edit given
  `field_name` to avoid malicious or erroneous use of it.
  [gbastien]
- Added new value `execute_tal_expression` for
  `MeetingConfig.onTransitionFieldTransforms.field_name`, this way it is now
  possible to define a TAL expression to execute after an item WF transition
  that will not change the content of a richtext field.
  [gbastien]

#### Products.MeetingCommunes (4.2.5 → 4.2.6)

#### Version 4.2.6 (2024-02-26)

- Import `get_person_from_userid` from `collective.contact.plonegroup.utils`
  instead `Products.PloneMeeting.utils`.
  [gbastien]

#### imio.actionspanel (1.64 → 1.65)

#### Version 1.65 (2024-02-08)

- Use `typeInfo.Title()` to get portal_type's title instead
  translating the `typeInfo.title`.
  [gbastien]

#### imio.annex (2.20 → 2.21)

#### Version 2.21 (2023-12-11)

- Use our own event `ConversionReallyFinishedEvent` instead
  collective.documentviewer's `ConversionFinishedEvent` because it is called
  when `converting` information is still not set back to `False` and we need
  to have this information when an annex is updated and conversion is run again
  because in this case, `successfully_converted` is still `True`.
  [gbastien]

#### imio.helpers (0.77 → 1.0.0rc1)

#### Version 1.0.0 (2024-09-16)

- Improved `emailer.send_email` to use send in place of securesend (not using queue).
  [sgeulette]
- Added `EMPTY_DATETIME` value that corresponds to `01/01/1950 at 12:00`.
  [gbastien]
- Improved batching module
  [sgeulette]
- Added `batching.can_delete_batch_files`
  [sgeulette]

#### Version 1.0.0rc1 (2024-02-08)

- Added "empty" variables to handle empty indexes searches.
  [sgeulette]


- Added `temp_disable_link` JS helper that will disable a link for 2 seconds
  and to avoid double clicks.
  [gbastien]


- Added batching module.
  [sgeulette]
- Fixed the way JS function `submitFormHelperOnsuccessDefault` manages
  returned result when it is a file, now we have a correct `filename`.
  [gbastien]
- Added transmogrifier Expression and Condition classes to log expression
  compilation or interpretation errors.
  [sgeulette]
- Removed `content.safe_encode` as already defined in `imio.pyutils`.
  Import it from `imio.pyutils` in `imio.helpers.content` for temporary backward
  compatibility, to be removed.
  [gbastien]
- Overrided `@@folder_contents` to make it work with `DashboardCollection`.
  [gbastien]
- Monkeypatched `plone.app.querystring.registryreader.getVocabularyValues`
  to keep vocabulary order onloy for Plone4, behavior is correct in Plone5+.
  Manage every `HAS_PLONE_X` values.
  [gbastien]


- Made compliant with Plone 4, Plone 5, Plone 6
  [boulch, laulaz, sgeulette]
- Require `pathlib2` in `setup.py`, backport `pathlib` for `py2.7`.
  [gbastien]
- Added `security.setup_app` to be used in run scripts.
  [sgeulette]
- Added `setup.load_xml_tool_only_from_package` to load only main tool xml file.
  [sgeulette]
- Added `setup.test_remove_gs_step` to remove a generic setup step.
  [sgeulette]
- Added `imio.helpers.YesNoForFacetedVocabulary`
  [sgeulette]
- Fixed `content.base_getattr` that was not returning the `default` if attribute
  not existing.
  [gbastien]

#### Version 0.80 (2023-12-11)

- Added parameter `with_user_id` to `content.get_user_fullname`, this will
  include `userid` in brackets in result like `Firstname Lastname (userid)`.
  [gbastien]
- Added parameter `userid` to `security.get_user_from_criteria`
  [sgeulette]

#### Version 0.79 (2023-11-28)

- Improved `security.get_user_from_criteria` to add email and description in ldap results.
  [sgeulette]
- Included Products.CMFCore permissions.zcml
  [sgeulette]

#### Version 0.78 (2023-10-27)

- Added `workflow.get_final_states` that will return a given WF final states.
  [gbastien]

#### imio.history (1.30 → 1.33)

#### Version 1.33 (2023-12-11)

- Added `utils.add_event_to_wf_history` to insert an event
  to the `workflow_history` of an element.
  [gbastien]

#### Version 1.32 (2023-11-27)

- In `IHDocumentBylineViewlet`, do not display creator if `show_history`
  is `False` as creator is part of the history.
  [gbastien]
- In `@@historyview`, display a `@@header` view under `History` title that will
  by default display the `prettylink` of the context, useful when displaying
  history in a popup from a dashboard containing plenty of elements.
  Added direct dependency on `imio.prettylink`.
  [gbastien]

#### Version 1.31 (2023-10-27)

- Added parameter `ignore_previous_event_actions=[]` to `utils.getLastAction`,
  this way when finding the last action in a history, it will check previous
  event action and continue if it is an action to ignore.
  [gbastien]

#### imio.migrator (1.33 → 1.34)

#### Version 1.34 (2024-02-08)

- Corrected `Migrator.cleanRegistries` to really save portal_setup changes.
  [sgeulette]

#### imio.prettylink (1.21 → 1.22)

#### Version 1.22 (2024-02-08)

- When displaying `contentIcon`, use `typeInfo.Title` method instead translating
  the `typeInfo.title` as `typeInfo.Title` manages various case where title is
  `unicode`, `string` or else.
  [gbastien]

#### imio.pyutils (0.31 → 1.0.0a1)

#### Version 1.0.0 (2024-03-05)

- Require `six>=1.16.0`.
  [sgeulette]
- Added `system.hashed_filename` to get a new filename differentiated by a hashed string.
  [sgeulette]

#### Version 1.0.0a1 (2024-02-08)

- Handled set in `load_var`.
  [sgeulette]
- Added `load_pickle` and `dump_pickle`
  [sgeulette]
- Improved `bs.is_empty`
  [sgeulette]

#### Version 1.0.0a (2023-11-28)

- Made py2 and py3 compliant
  [sgeulette]
- Improved `utils_safe_encode`
  [sgeulette]
- Added `bs.is_empty` function.
  [sgeulette]
- Added `bs.remove_some_childrens` function.
  [sgeulette]
- Added `bs.replace_strings_by_pattern` function
  [sgeulette]
- Added `exclude_patterns` parameter in `system.read_recursive_dir`
  [sgeulette]

#### collective.behavior.internalnumber (0.2 → 0.3)

#### Version 0.3 (2023-11-27)

- Removed catalog metadata `internal_number`, added upgrade step to 1001.
  [gbastien]

#### collective.contact.plonegroup (1.47 → 1.48)

#### Version 1.48 (2024-02-19)

- Added `behaviors.IPlonegroupUserLink` with userid and primary_organization fields.
  [sgeulette]
- Added `utils.get_person_from_userid` and `utils.get_persons_from_userid`
  [sgeulette]

#### collective.dms.scanbehavior (1.3 → 1.3.0)

*No changelog entries found.*

#### collective.eeafaceted.z3ctable (2.25 → 2.26)

#### Version 2.26 (2023-11-27)

- Take into account `VocabularyColumn.ignored_value` in `AbbrColumn`.
  [gbastien]

#### collective.iconifiedcategory (0.60 → 0.64)

#### Version 0.64 (2024-02-08)

- Added `IExcludeFromNavigation` behavior on `ContentCategoryConfiguration` type.
  [sgeulette]
- Corrected bad step dependency
  [sgeulette]

#### Version 0.63 (2024-01-02)

- Added `get_` and `set_` methods for settings registry records in `config.py`.
  [gbastien]

#### Version 0.62 (2023-12-11)

- Fixed `CategorizedObjectPreviewAdapter.status` when an existing element is updated.
  [gbastien]

#### Version 0.61 (2023-11-27)

- Simplified `CategorizedChildView.has_elements_to_show`.
  [gbastien]

#### collective.js.tooltipster (1.7 → 1.8)

#### Version 1.8 (2024-02-08)

- Added `arrow` option in `tooltipster_helper`.
  [sgeulette]

#### imio.pm.locales (4.2.8 → 4.2.15)

#### Version 4.2.15 (2024-02-26)

- Adapted french translations for `considered_not_given_hidden_during_redaction`
  and `hidden_during_redaction`.
  [gbastien]
- Adapted french translations for `MeetingConfig.onMeetingTransitionItemActionToExecute`.
  [gbastien]
- Fixed typo in `wa_postpone_next_meeting_keep_internal_number` french translation.
  [gbastien]

#### Version 4.2.14 (2024-02-08)

- Added translations for `MeetingItemRecurring` and `MeetingItemTemplate`,
  this prepare removal of every `Meeting/MeetingItem` portal_types translations.
  [gbastien]
- Added translations for `MeetingConfig.itemWFValidationLevels.groups_managing_item`.
  [gbastien]

#### Version 4.2.13 (2024-01-31)

- Adapted translations for `MeetingConfig.onTransitionFieldTransforms`.
  [gbastien]

#### Version 4.2.12 (2024-01-11)

- Adapted translations for the `Export PDF` action on item.
  [gbastien]

#### Version 4.2.11 (2024-01-02)

- Accurate french translation for `help_given_on_before_started_on`.
  [gbastien]
- Added translations for the `Export PDF` action on item.
  [gbastien]
- More accurate french translation for `copy_groups_help_msg`.
  [gbastien]

#### Version 4.2.10 (2023-12-11)

- Added translations related to new `advice_hide_during_redaction_history`.
  [gbastien]
- Added translation for `No vote for following ${number} item(s)`.
  [gbastien]
- Added translation for faceted filter `Title only`.
  [gbastien]
- Removed translations for the `add_advicecreated_state` WFA.
  [gbastien]

#### Version 4.2.9 (2023-11-27)

- Adapted translations for item mail events `lateItem`, `itemUnpresented`,
  `itemDelayed`, `itemPostponedNextMeeting`, `returnedToProposingGroup`,
  `returnedToMeetingManagers` to include last WF action author and comment.
  Added translation for new item mail notification
  `event_item_postponed_next_meeting_owner`.
  [gbastien]
- Added translations for `ToolPloneMeeting.advisersConfig`.
  [gbastien]
- Added translation for `Everyone`.
  [gbastien]
- Added translation for `static_item_meeting_deadline_date`.
  [gbastien]
- Added translation for `annexes_preview_config`.
  [gbastien]
- Added translations for new WFA `wa_postpone_next_meeting_keep_internal_number`
  and `wa_postpone_next_meeting_transfer_annex_scan_id`.
  [gbastien]

#### imio.pm.ws (3.8 → 3.9)

#### Version 3.9 (2023-12-11)

- Adapted code as `Products.PloneMeeting.utils.add_wf_history_action` was moved
  to `imio.history.utils.add_event_to_wf_history` and `ToolPloneMeeting.getUserName`
  is removed, we use `imio.helpers.content.get_user_fullname` instead.
  [gbastien]

#### plonemeeting.restapi (2.2 → 2.3)

#### Version 2.3 (2023-12-11)

- Adapted code as `Products.PloneMeeting.utils.add_wf_history_action` was moved
  to `imio.history.utils.add_event_to_wf_history` and
  `ToolPloneMeeting.getAdvicePortalTypes` and
  `ToolPloneMeeting.getAdvicePortalTypeIds` were moved to utils.
  [gbastien]

#### plonetheme.imioapps (2.43 → 2.45)

#### Version 2.45 (2024-01-02)

- Fixed change introduced in release `2.44` with tag `h1` in overlays that
  was impacting other overlays.
  Moreover removed border bottom of `History` title in history overlay.
  [gbastien]

#### Version 2.44 (2023-11-27)

- Now that element's title (pretty link) is displayed in `@@historyview`,
  display `h1` in overlay the same size it is display out of an overlay.
  [gbastien]

## Release 4.2.23

**Date:** 2024-01-25

### Package Updates

#### Products.PloneMeeting (4.2.8 → 4.2.8.2)

*No changelog entries found.*

## Release 4.2.22

**Date:** 2024-01-16

### Package Updates

#### Products.PloneMeeting (4.2.9b9 → 4.2.8)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2.6b7 → 4.2.5)

*No changelog entries found.*

#### imio.annex (2.21 → 2.20)

*No changelog entries found.*

#### imio.helpers (0.80 → 0.77)

*No changelog entries found.*

#### imio.history (1.33 → 1.30)

*No changelog entries found.*

#### collective.behavior.internalnumber (0.3 → 0.2)

*No changelog entries found.*

#### collective.dms.scanbehavior (1.3.0 → 1.3)

*No changelog entries found.*

#### collective.eeafaceted.z3ctable (2.26 → 2.25)

*No changelog entries found.*

#### collective.iconifiedcategory (0.63 → 0.60)

*No changelog entries found.*

#### imio.pm.locales (4.2.13 → 4.2.8)

*No changelog entries found.*

#### imio.pm.ws (3.9 → 3.8)

*No changelog entries found.*

#### plonemeeting.restapi (2.3 → 2.2)

*No changelog entries found.*

#### plonetheme.imioapps (2.45 → 2.43)

*No changelog entries found.*

## Release 4.2.22b1

**Date:** 2024-01-31

### Package Updates

#### Products.PloneMeeting (4.2.8 → 4.2.9b9)

#### Version 4.2.9 (2024-06-10)

- In `EveryAnnexTypesVocabulary` use `content_category` icon image scale
  instead `portal_url.getRelativeUrl` so it is cached.
  [gbastien]
- Execute `upgrade_step_4211_add_item_widgets.xml` adding faceted criterion
  `title only` again in upgrade to `4214` as it was not in
  `default_dashboard_items_widgets.xml`, new `MeetingConfig` added since
  profile version `4211` are missing this criterion.
  [gbastien]
- Completed `print_votes` so it manages every `vote_values`
  (`does_not_vote`, `not_found`, `invalid`, `blank`).
  Adapted parameter `single_vote_value` so we can define a single value or
  a different value for each `vote_values`.
  Adapted parameter `include_voters=False` that maye be False/True or a list of
  vote values.
  Added parameter `include_voters_percent_treshold=100` that is an integer value
  from 0 to 100 that will display voters if ratio between number of voters and
  total voters exceeds the treshold.
  [gbastien]
- Added field `MeetingItem.restrictedCopyGroups`, a secondary `copyGroups` field
  where we can define other groups having access to item in other (later) states.
  [gbastien]
- Now every deletion is protected by `IContentDeletable`, including default
  Plone deletion using `manage_delObjects`.
  [gbastien]
- Fixed item number not saved when using `Disk` icon to change item number
  on meeting view when item number is a subnumber.
  [gbastien]
- Fixed validation of meeting signatories when creating a meeting, it was possible
  to create a meeting with several signatories using same signature number.
  [gbastien]
- Added per power observer complementary workflow adaptation to base
  `hide_decisions_when_under_writing` to let the selected power observers
  have access to the item decision.
  [gbastien]
- Improve `view.print_attendees_by_type` to be able to customize the in and out
  count more.
  [aduchene]
- Allow to use OrderedDict in POD templates.
  [aduchene]
- Fixed attendees statistics wrong absent/excused computation in sheet by meeting.
  [gbastien]
- Integrate `imio.webspellchecker` to replace `Scayt` for `CKEditor`.
  As `WSC` is started when focus is set in `CKEditor` field, set focus on
  field when using quick edit.
  [gbastien]
- Avoid double click on POD template mailing list.
  [gbastien]
- Generate `Meeting/MeetingItem` portal_type title based on `MeetingConfig`
  title instead translating it.
  [gbastien]
- Optimized `@@load_item_assembly_and_signatures` especially when several
  voters (50) and votes for an item (25).
  [gbastien]
- Fixed encode votes for several items failed when there was a `no_vote` item
  in the way.
  [gbastien]

#### Version 4.2.9rc6 (2024-04-10)

- Moved field `Meeting.pre_observations` before `Meeting.observations`.
  [gbastien]
- Make `test_pm_WFA_availableWFAdaptations` more robust by generating the
  `presented_item_back_to_` WF adaptations as it relies on defined
  `MeetingConfig.itemWFValidationLevels`.
  [gbastien]
- Make tests using `utils.set_field_from_ajax` more robust by using field
  `description` instead `decision` as in some case (subplugin), `decision`
  field is not writable.
  [gbastien]
- Do not automatically reinitialize the delay of an advice during the
  `MeetingConfig.transitionsReinitializingDelays` if delay was timed out,
  this will have to be done manually.
  [gbastien]
- Renamed `test_pm_WFA_waiting_advices` to `test_pm_WFA_waiting_advices_base`
  so it can be executed separately than other `test_pm_WFA_waiting_advices_`
  tests.
  Completed `test_pm_ItemActionsPanelCachingProfiles` to check when reviewer
  may also edit crated item (when using `extra_suffixes`), this way we may
  remove `_reviewers_may_edit_itemcreated` helper.
  [gbastien]
- Fixed `test_pm_ItemMailNotificationLateItem` when called from subplugins.
  [gbastien]
- Make `test_pm_Validate_itemWFValidationLevels_removed_depending_used_state_item`
  and `test_pm_SearchItemsToCorrectToValidateOfEveryReviewerGroups` more robust
  when called from subplugin.
  [gbastien]
- Adapted `Products.PloneMeeting.vocabularies.advicetypesvocabulary`, used in
  advice types faceted filter to take into account
  `ToolPloneMeeting.advisersConfig.advice_types`.
  [gbastien]
- Add two types of email notifications to suffixes about given advices.
  Added upgrade step to 4214 to update `MeetingConfig.mailItemEvents`.
  [aduchene]
- Add a notification to power observers about late items.
  [aduchene]
- When `MeetingConfig.mailMode` is set to `test`, display the sent mail `subject`
  and `recipients` in a portal message.
  [gbastien]
- Do not break in `MeetingConfig` POD templates when some reusable POD templates
  were deleted or marked no more reusable.
  [gbastien]
- Import `safe_encode` from `imio.pyutils` instead `imio.helpers`.
  [gbastien]
- Now that `@@folder_contents` works on `DashboardCollection`,
  added `test_pm_Folder_contents` to confirm it.
  [gbastien]
- Added `tobytes` and `fileSize` from `Products.CPUtils` to `safe_utils`, this
  is necessary to convert `portal_catalog` `getObjSize` format to `bytes` and
  `bytes` to a human readable format.
  [gbastien]
- Back to previous behavior in `utils._sendMail`, when sending an email
  with attachment, send it only one time to every recipients instead sending
  it one time by recipient.
  [gbastien]
- Avoid vocabulary `AskedAdvicesVocabulary` being empty when cached because
  `MeetingConfig` could not be obtained.
  [gbastien]
- Display `MeetingConfig.usingGroups` field on `MeetingConfig` view home page
  under `Groups and users` to identify easily a MeetingConfig using this parameter.
  [gbastien]
- Added parameters `withItemNumber=False` and `withItemReference=False` to
  `MeetingItem.Title` to have the item title prefixed with item reference
  and/or item number.
  [gbastien]
- Adapted `utils._sendMail` to use `bcc` (`blind carbon copy`) when sending
  an email with attachment (one email sent to several recipients).
  [gbastien]
- Display `TAL condition` by default on `MeetingConfig` view in
  `POD templates` section.
  [gbastien]

#### Version 4.2.9rc5 (2024-03-14)

- Added upgrade step to 4213 to fix POD templates that were using
  `.adapted().getCertifiedSignatures()` to `.getCertifiedSignatures()`,
  `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]

#### Version 4.2.9rc4 (2024-03-14)

- Added `org_uid` to elements available when evaluating the TAL expression on an
  organization to compute `as_copy_groups_on`.
  [gbastien]
- Adapted `MeetingCategory.is_selectable`, will no more be selectable if
  functionnality not enabled in `MeetingConfig`.
  [gbastien]
- Added warning on MeetingConfig view in the POD templates section to warn user
  to edit templates only if relevant and to never user MS Word.
  [gbastien]
- Avoid `UnicodeDecodeError` in `ConfigHideHistoryTosVocabulary`.
  [gbastien]
- `MeetingItem.getCertifiedSignatures` is no more an adaptable method.
  [gbastien]
- Moved field `advice.advice_reference` under `advice.advice_accounting_commitment`
  so `RichText` fields are grouped together.
  Display `advice_reference` in advice tooltipster when not empty.
  [gbastien]

#### Version 4.2.9rc3 (2024-03-05)

- Fixed custom advice WF UI:

  - do not display `given_by` information when using the default advice workflow;
  - in `onAdviceTransition` event, notify `AdviceAfterTransitionEvent` after
    `hidden_during_redaction` auto set to `False` management;
  - adapted import_data to manage `advisersConfig`.

  [gbastien]
- Display advice type id when using vocabulary `ConfigAdviceTypes` in the configuration.
  [gbastien]
- Removed redirect from `ChangeItemCompletenessView._changeCompleteness`, this
  is already managed in the `__call__` method, this avoid a redirect when calling
  `_changeCompleteness` directly from another code, like an event.
  [gbastien]
- Added some padding top of custom advice message on advice view.
  [gbastien]
- Optimized `MeetingItem._updateAdvices` to avoid several computation of
  advisers when using inherited advices. This also fixes problem with optional
  key that was wrongly initialized for inherited advices.
  [gbastien]
- Removed unused vocabularies `PMEveryCategoryVocabulary` and
  `PMEveryCategoryTitleVocabulary`.
  [gbastien]

#### Version 4.2.9rc2 (2024-02-26)

- Added helper `MeetingConfig.get_transitions_to_close_a_meeting`.
  Removed adaptable method `MeetingItemWorkflowActions._latePresentedItemTransitions`
  no more necessary as this is managed automatically now based on
  `MeetingConfig.onMeetingTransitionItemActionToExecute`.
  [gbastien]
- Added `imio.helpers.date.formatDate` to `safe_utils` so it is available in
  TAL expressions.
  [gbastien]
- Make sure `print_votes` always return a string when `render_as_html=True`.
  [gbastien]
- Removed field `IPMPerson.userid`, instead use behavior
  `collective.contact.plonegroup.behaviors.IPlonegroupUserLink` that will add
  fields `userid` and `primary_organization`.  We use `primary_organization` as
  a way to manage default `proposingGroup` when creating an item.
  [gbastien]
- Fixed `utils._sendMail` to avoid `UnicodeDecodeError`.
  Also refactored it so the loop on recipients is managed by `utils._sendMail`
  and one mail is sent by recipient in any case (attachments or not).
  [gbastien]
- Use ZLogHandler in `ToolPloneMeeting.update_all_local_roles`.
  [aduchene]

#### Version 4.2.9rc1 (2024-02-08)

- Adapted portal tabs sub menu styling to make more `sub menu`.
  [gbastien]
- Fixed critical bug while sending mail that was preventing to use the MailHost
  mail_queue because using `secureSend` from `Products.CMFPlone` that is
  deprecated and that use `immediate=True`.
  Now emails will be correctly using the mail_queue and start it when necessary.
  [gbastien]
- In `utils.updateAnnexesAccess`, make sure we do not acquire attribute
  `categorized_elements` or update is done several times, this is the case when
  called on an advice, the parent item attribute was used.
  [gbastien]
- Prevent a siteadmin from renaming an item linked to a meeting (an item that
  is no more in it's WF initial state) or it breaks the link with the meeting.
  [gbastien]

#### Version 4.2.9b9 (2024-01-31)

- Make the advice `given_on` date use final WF state when using a custom WF.
  [gbastien]

#### Version 4.2.9b8 (2024-01-18)

- Do not `show_advice_on_final_wf_transition` when item is set in a wf state
  in which advice can not be edited anymore if advice did not reached it's final
  state (when using advice custom worklow).
  [gbastien]

#### Version 4.2.9b7 (2024-01-11)

- Added `Export PDF` action to `MeetingConfig.itemActionsColumnConfig`.
  [gbastien]

#### Version 4.2.9b6 (2024-01-11)

- Removed constant `config.ADVICE_STATES_ALIVE`, it is now managed automatically
  by `utils.get_advice_alive_states` and it will ne more be necessary to
  override it in custom profiles.
  [gbastien]
- In tests, use `imio.helpers.content.richtextval` everywhere a `RichTextValue` is used.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]

#### Version 4.2.9b5 (2024-01-02)

- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `Export PDF` action on item to be able to export in a single PDF file
  several selected PDF generated POD templates and PDF annexes.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Fixed CSS of advice popup label when very long.
  [gbastien]
- When `copyGroups` have access to item, highlight full `Copy groups` label in green.
  [gbastien]

#### Version 4.2.9b4 (2023-12-11)

- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]

#### Version 4.2.9b3 (2023-11-27)

- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]

#### Version 4.2.9b2 (2023-11-27)

- Display last transition actor and comment in item mail notifications for mail events:

  - `lateItem`;
  - `itemUnpresented`;
  - `itemDelayed`;
  - `itemPostponedNextMeeting`;
  - `returnedToProposingGroup`;
  - `returnedToMeetingManagers`.

  Added new item mail event `itemPostponedNextMeetingOwner`
  (in addition to `itemPostponedNextMeeting`).
  [gbastien]
- Fixed `ItemOptionalAdvicesVocabulary` caching to take into account delay aware
  advisers in cachekey as it is computed and depends on context.
  Fixed also a bug when some `__userid__` selected values were no more in the
  vocabulary with other values still in the vocabulary.
  [gbastien]
- Added `MeetingConfig.show_copy_groups_search` that is used to protect
  copyGroups related searches.
  [gbastien]
- Fixed `PMCategorizedChildView.__call___`, if no categorized elements,
  do not return just [] but the parameter `show_nothing` value,
  as it is rendered differently if True or False.
  [gbastien]
- Make `MeetingItem.meetingDeadlineDate` displayable in dashboards as static info
  (always visible in the item `Title` column).
  [gbastien]
- Static info `Item reference` is now selectable in the
  `MeetingConfig.availableItemsListVisibleColumns` as item reference may now be
  set before item is inserted into a meeting.
  [gbastien]
- Added `static_labels` and `static_item_reference` to the selectable values for
  `MeetingConfig.itemsVisibleFields` and `MeetingConfig.itemsNotViewableVisibleFields`.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_keep_internal_number`
  that will keep the `MeetingItem.internal_number` when `postpone_next_meeting`
  an item as the new item is somewhat the same presented again in another meeting.
  [gbastien]
- Added complementary WFAdaptation `postpone_next_meeting_transfer_annex_scan_id`
  that will keep the annexes with a `scan_id` but transfer this `scan_id` from
  original annexes (where `scan_id` is set to None) to new annexes.
  [gbastien]
- Added `advice_hide_during_redaction_history` to store
  `advice.advice_hide_during_redaction` changes by user.
  [gbastien]
- Simplified `ToolPloneMeeting` to be able to move it to a registry adapter as
  light as possible, so remove most functionnalities from it:

  - Moved `ToolPloneMeeting.showMeetingView` to `MeetingFacetedView.show_page`
    as it is only used there;
  - Removed `TooPloneMeeting.getColoredLink`, use `MeetingItem.getPrettyLink`;
  - Moved `ToolPloneMeeting.getMailRecipient` to utils;
  - Moved `ToolPloneMeeting.getAdvicePortalTypes` and
    `ToolPloneMeeting.getAdvicePortalTypeIds` to utils;
  - Moved `ToolPloneMeeting.getAvailableMailingLists` to utils;
  - Removed no more used `versions_history_form.pt`;
  - Moved `ToolPloneMeeting.isPowerObserverForCfg` to
    `utils.isPowerObserverForCfg`;
  - Replaced `ToolPloneMeeting.getUserName` by
    `imio.helpers.content.get_user_fullname` everywhere it was used.

  [gbastien]
- Adapted `DisplayMeetingItemVoters` helper view on meeting to display items
  with `No vote` separately than items with `public` and `secret` votes and to
  not display it in non voted items anymore.
  [gbastien]
- Added faceted filter criterion `Item title only` to query items on
  items's title only using the `Title` index.
  [gbastien]
- When using `MeetingConfig.computeItemReferenceForItemsOutOfMeeting`, do not clear
  item reference when meeting back to `created` or when item back to `validated`.
  Renamed `MeetingItem.mustShowItemReference` to `MeetingItem.show_item_reference`.
  [gbastien]
- In dashboards displaying items, display `Proposing group` before `Category`
  and `Classifier`.
  [gbastien]
- Fixed update `categorized_elements` of advices when advice moved as
  stored path changed (when advice is given on an item that is `itemcreated` and
  that is renamed).
  [gbastien]
- Make sure every item related searches (Collection) use `sort_on` modified
  as this is not visible in the application because faceted `sort_on` overrides
  it but it is now taken into account when using restapi with a `base_search_uid`.
  [gbastien]

#### Version 4.2.9b1 (2023-10-27)

- Added advanced advice management using `ToolPloneMeeting.advisersConfig`:

  - possible to associate a new advice `portal_type` to some organizations;
  - reworked advice infos template to add more CSS classes to additional infos;
  - display the `Advice given by` information;
  - added possibility to hide advice history to power observers and to everyone
    and to hide meeting history to powerobservers.

  [gbastien]
- Use `CompoundCriterion` adapter `living-items` for the `searchlivingitems`
  Collection so selected states are always correct if item workflow
  configuration changed.
  [gbastien]
- When advice is `asked_again` display left delay correctly, full delay is displayed
  when advice is supposed given, but when is it `asked_again` it is not the case.
  [gbastien]
- Added `sortable` functionnality to the `PMCheckBoxWidget`, use it in the item
  `Export PDF` form to be able to reorder exported elements.
  [gbastien]
- Mail notifications `adviceEdited` and `adviceEditedOwner` are no more sent
  if advice is hidden during redaction.
  [gbastien]
- Fixed `AdvicesIcons.get_advice_given_by` to only return a value when using
  custom WF (more than one initial state) and if WF reached it's final state.
  [gbastien]
- Fixed `MeetingConfig.listTransitionsUntilPresented` that was raising
  `UnicodeDecodeError` now that we use unicode arrow in term title.
  Use unicode arrow in `utils.get_dx_attrs` when `as_display_list=True`.
  [gbastien]
- Check user is creator in item `actions_panel` caching invalidation.
  [gbastien]
- Display `created/modified` dates on `MeetingConfig view` for `categories`,
  `classifiers`, `recurring items`, `searches` and `pod templates`.
  [gbastien]
- Added in and out count to `print_attendees_by_type`.
  [aduchene]
- In `utils.set_field_from_ajax`, check again that user may actually edit given
  `field_name` to avoid malicious or erroneous use of it.
  [gbastien]
- Added new value `execute_tal_expression` for
  `MeetingConfig.onTransitionFieldTransforms.field_name`, this way it is now
  possible to define a TAL expression to execute after an item WF transition
  that will not change the content of a richtext field.
  [gbastien]

#### Products.MeetingCommunes (4.2.5 → 4.2.6b7)

#### Version 4.2.6 (2024-02-26)

- Import `get_person_from_userid` from `collective.contact.plonegroup.utils`
  instead `Products.PloneMeeting.utils`.
  [gbastien]

#### Version 4.2.6rc1 (2024-02-08)

- Added parameter `ignore_not_given_advice=False` to
  `CustomMeetingItem.showFinanceAdviceTemplate`, when `True`, this will hide
  the POD template when advice is `not_given` or `asked_again`.
  [gbastien]

#### Version 4.2.6b7 (2024-01-31)

- Added `test_pm_Show_advice_on_final_wf_transition_when_item_in_advice_not_giveable_state`
  that will test that when item is set to a state in which advice is no more
  editable, `advice.advice_hide_during_redaction` is not set back to `True`
  if advice was not in it's workflow final state (when using advice custom workflow).
  [gbastien]
- Adapted `test_Get_advice_given_by` to check that `get_advice_given_on` is
  the advice WF `signFinancialAdvice` transition date when using a custom WF.
  [gbastien]

#### Version 4.2.6b6 (2024-01-11)

- Adapted code to use `imio.helpers.content.richtextval` instead `RichTextValue` when possible.
  [gbastien]

#### Version 4.2.6b5 (2024-01-02)

- Added translations for the `add_advicecreated_state` WFA.
  [gbastien]
- Every item related search (Collection) use `sort_on` `modified` instead `created`.
  [gbastien]

#### Version 4.2.6b4 (2023-12-11)

- CSS, color in blue state `financial_advice_signed` in advice history.
  [gbastien]
- Adapted code as `ToolPloneMeeting.getUserName` is replaced by
  `imio.helpers.content.get_user_fullname` and
  `ToolPloneMeeting.isPowerObserverForCfg` is moved to
  `utils.isPowerObserverForCfg`.
  [gbastien]

#### Version 4.2.6b3 (2023-11-27)

- Added parameter `ignore_advice_hidden_during_redaction=False` to
  `CustomMeetingItem.showFinanceAdviceTemplate`, when `True`, this will hide
  the POD template when advice is hidden during redaction except if member is
  `MeetingManager` or in the advice `_advisers` group.
  [gbastien]

#### Version 4.2.6b2 (2023-11-27)

- Move back `add_advicecreated_state` advice WFA related code from `PloneMeeting`.
  [gbastien]
- Fixed `meetingadvicefinancs` `portal_type.allowed_content_types` install.
  [gbastien]
- Completed translations of finances advices types.
  [gbastien]

#### Version 4.2.6b1 (2023-10-27)

- Adapted code now that custom advice portal_types is managed by
  `ToolPloneMeeting.advisersConfig`:

  - Added new advice finances WF `meetingadvicefinancessimple_workflow`;
  - Fixed tests as `MeetingConfig.listWorkflowAdaptations` was removed.

  [gbastien]
- Added `Export users/groups` dashboard template for contacts in `examples_fr` profile.
  [gbastien]
- Updated `recapitulatif-tb.ods` to use `appy.pod` instruction `do cell from+ xhtml(...)`
  instead `view.display_html_as_text`.
  [gbastien]
- Fixed `CustomMeetingConfig.getUsedFinanceGroupIds` that was not working
  for auto asked advices.
  [gbastien]

#### imio.annex (2.20 → 2.21)

#### Version 2.21 (2023-12-11)

- Use our own event `ConversionReallyFinishedEvent` instead
  collective.documentviewer's `ConversionFinishedEvent` because it is called
  when `converting` information is still not set back to `False` and we need
  to have this information when an annex is updated and conversion is run again
  because in this case, `successfully_converted` is still `True`.
  [gbastien]

#### imio.helpers (0.77 → 0.80)

#### Version 0.80 (2023-12-11)

- Added parameter `with_user_id` to `content.get_user_fullname`, this will
  include `userid` in brackets in result like `Firstname Lastname (userid)`.
  [gbastien]
- Added parameter `userid` to `security.get_user_from_criteria`
  [sgeulette]

#### Version 0.79 (2023-11-28)

- Improved `security.get_user_from_criteria` to add email and description in ldap results.
  [sgeulette]
- Included Products.CMFCore permissions.zcml
  [sgeulette]

#### Version 0.78 (2023-10-27)

- Added `workflow.get_final_states` that will return a given WF final states.
  [gbastien]

#### imio.history (1.30 → 1.33)

#### Version 1.33 (2023-12-11)

- Added `utils.add_event_to_wf_history` to insert an event
  to the `workflow_history` of an element.
  [gbastien]

#### Version 1.32 (2023-11-27)

- In `IHDocumentBylineViewlet`, do not display creator if `show_history`
  is `False` as creator is part of the history.
  [gbastien]
- In `@@historyview`, display a `@@header` view under `History` title that will
  by default display the `prettylink` of the context, useful when displaying
  history in a popup from a dashboard containing plenty of elements.
  Added direct dependency on `imio.prettylink`.
  [gbastien]

#### Version 1.31 (2023-10-27)

- Added parameter `ignore_previous_event_actions=[]` to `utils.getLastAction`,
  this way when finding the last action in a history, it will check previous
  event action and continue if it is an action to ignore.
  [gbastien]

#### collective.behavior.internalnumber (0.2 → 0.3)

#### Version 0.3 (2023-11-27)

- Removed catalog metadata `internal_number`, added upgrade step to 1001.
  [gbastien]

#### collective.dms.scanbehavior (1.3 → 1.3.0)

*No changelog entries found.*

#### collective.eeafaceted.z3ctable (2.25 → 2.26)

#### Version 2.26 (2023-11-27)

- Take into account `VocabularyColumn.ignored_value` in `AbbrColumn`.
  [gbastien]

#### collective.iconifiedcategory (0.60 → 0.63)

#### Version 0.63 (2024-01-02)

- Added `get_` and `set_` methods for settings registry records in `config.py`.
  [gbastien]

#### Version 0.62 (2023-12-11)

- Fixed `CategorizedObjectPreviewAdapter.status` when an existing element is updated.
  [gbastien]

#### Version 0.61 (2023-11-27)

- Simplified `CategorizedChildView.has_elements_to_show`.
  [gbastien]

#### imio.pm.locales (4.2.8 → 4.2.13)

#### Version 4.2.13 (2024-01-31)

- Adapted translations for `MeetingConfig.onTransitionFieldTransforms`.
  [gbastien]

#### Version 4.2.12 (2024-01-11)

- Adapted translations for the `Export PDF` action on item.
  [gbastien]

#### Version 4.2.11 (2024-01-02)

- Accurate french translation for `help_given_on_before_started_on`.
  [gbastien]
- Added translations for the `Export PDF` action on item.
  [gbastien]
- More accurate french translation for `copy_groups_help_msg`.
  [gbastien]

#### Version 4.2.10 (2023-12-11)

- Added translations related to new `advice_hide_during_redaction_history`.
  [gbastien]
- Added translation for `No vote for following ${number} item(s)`.
  [gbastien]
- Added translation for faceted filter `Title only`.
  [gbastien]
- Removed translations for the `add_advicecreated_state` WFA.
  [gbastien]

#### Version 4.2.9 (2023-11-27)

- Adapted translations for item mail events `lateItem`, `itemUnpresented`,
  `itemDelayed`, `itemPostponedNextMeeting`, `returnedToProposingGroup`,
  `returnedToMeetingManagers` to include last WF action author and comment.
  Added translation for new item mail notification
  `event_item_postponed_next_meeting_owner`.
  [gbastien]
- Added translations for `ToolPloneMeeting.advisersConfig`.
  [gbastien]
- Added translation for `Everyone`.
  [gbastien]
- Added translation for `static_item_meeting_deadline_date`.
  [gbastien]
- Added translation for `annexes_preview_config`.
  [gbastien]
- Added translations for new WFA `wa_postpone_next_meeting_keep_internal_number`
  and `wa_postpone_next_meeting_transfer_annex_scan_id`.
  [gbastien]

#### imio.pm.ws (3.8 → 3.9)

#### Version 3.9 (2023-12-11)

- Adapted code as `Products.PloneMeeting.utils.add_wf_history_action` was moved
  to `imio.history.utils.add_event_to_wf_history` and `ToolPloneMeeting.getUserName`
  is removed, we use `imio.helpers.content.get_user_fullname` instead.
  [gbastien]

#### plonemeeting.restapi (2.2 → 2.3)

#### Version 2.3 (2023-12-11)

- Adapted code as `Products.PloneMeeting.utils.add_wf_history_action` was moved
  to `imio.history.utils.add_event_to_wf_history` and
  `ToolPloneMeeting.getAdvicePortalTypes` and
  `ToolPloneMeeting.getAdvicePortalTypeIds` were moved to utils.
  [gbastien]

#### plonetheme.imioapps (2.43 → 2.45)

#### Version 2.45 (2024-01-02)

- Fixed change introduced in release `2.44` with tag `h1` in overlays that
  was impacting other overlays.
  Moreover removed border bottom of `History` title in history overlay.
  [gbastien]

#### Version 2.44 (2023-11-27)

- Now that element's title (pretty link) is displayed in `@@historyview`,
  display `h1` in overlay the same size it is display out of an overlay.
  [gbastien]

## Release 4.2.21

**Date:** 2023-10-27

### Package Updates

#### Products.PloneMeeting (4.2.4 → 4.2.8)

#### Version 4.2.8 (2023-10-27)

- Added new advice type `Read`.
  [gbastien]
- Added a new utils `set_internal_number` to be able to change the `internal_number`.
  [aduchene]
- Removed `config.BARCODE_INSERTED_ATTR_ID`, we do not use it anymore to check
  if a barcode was inserted, we rely on the `scan_id`.
  Added upgrade step to 4210.
  [gbastien]
- Added holidays for 2024. Completed upgrade step to 4210.
  [aduchene]

#### Version 4.2.7 (2023-10-19)

- Override the `org_pretty_link_with_additional_infos` column used in contacts
  dashboards to reload widget of `held_position.position_type` field as the
  vocabulary is gender aware, values may change from a `held_position` to another.
  [gbastien]
- Load `communesplone.layout` zcml sooner so overrided translations are loaded,
  this is especially the case for `label_by_author` translation.
  [gbastien]
- Fixed `ItemOptionalAdvicesVocabulary` to manage correctly missing terms when
  it involves userids. Added caching as it is used when editing an item.
  [gbastien]
- Added `imio.helpers.xhtml.unescape_html` to `safe_utils` so it is available in
  TAL expressions, this will decode an HTML content containing HTML entities.
  [gbastien]
- Added new optional field `MeetingItem.meetingDeadlineDate` and
  the related faceted dashboard column.
  [gbastien]
- Added 2 new advice types `negative_with_remarks` and `back_to_proposing_group`.
  [gbastien]

#### Version 4.2.6 (2023-09-21)

- Fixed migration to 4209:

  - Remove broken annexes before upgrading `collective.iconifiedcategory`;
  - Migrate `cfg/getUseCopies` in TAL expressions;
  - Upgrade `imio.annex` before updating annex `portal_type`.

  [gbastien]
- Advice historized data preview that was only accessible to `MeetingManagers`
  is now accessible to `advisers` of the historized data advice and
  `proposingGroup` members.
  [gbastien]
- Make sure `data_changes` history does not use `highlight_last_comment` or
  it drastically slows down item view when used.
  [gbastien]
- Protect history icon in advice popup the same way the history link
  is protected on the advice view.
  [gbastien]
- Use `imio.history.utils.add_event_to_history` to manage new history event for
  item `completeness` and `emergency` changes. In views displaying the history
  use the adapter to get the history instead accessing the stored attribute.
  [gbastien]
- CSS improvements:

  - Refreshed meeting select dropdown;
  - For long multiselect fields for which max height is fixed to avoid a too
    long field, fixed the field label so it is always visible.

  [aduchene, gbastien]

#### Version 4.2.5 (2023-09-12)

- Make the `Change groups in charge` batch action available on meetings.
  [gbastien]
- Removed monkeypatch for `plone.restapi.services.Service` that was done to
  display input/output logging as this was moved to `imio.restapi`.
  [gbastien]
- Added possibility to enable annex preview on a per annex category basis.
  When enabled, annex may only be downloaded by proposing group members and
  (Meeting)Managers.
  [gbastien]
- Added possibility to not keep some annexes when item sent to another MC.
  Needed to refactor override of `ContentCategory`,
  moved back code from `imio.zamqp.pm`.
  Added validation for `ContentCategory.other_mc_correspondences`.
  [gbastien]
- By default, when an item sent to another MC, annexes with a `scan_id`
  are not kept. Now annexes with a `scan_id` will be kept if a
  `ContentCategory.other_mc_correspondences` is defined
  (but `scan_id` is set to `None`).
  [gbastien]
- When removing an item from a meeting, make sure item `UID` is removed from
  `Meeting.item_attendees_positions` and `Meeting.item_attendees_order`.
  This rely now on `config.MEETING_ATTENDEES_ATTRS` that makes sure that every
  meeting attendees custom attributes are cleaned when item is removed.
  [gbastien]
- Display the spinner on annex under conversion when `to_print` was set to True.
  Added `View preview` action on annex and annexDecision that is displayed when
  a preview is available for the annex.
  [gbastien]
- Added batch action to change items copy groups:

  - Removed field `MeetingConfig.useCopies` and `MeetingItem.isCopiesEnabled`,
    field `MeetingItem.copyGroups` is now an optional field managed by
    `MeetingConfig.usedItemAttributes`;
  - Fixed `UpdateGroupsInChargeBatchActionForm`, make sure item `local_roles`
    are correct after groups in charge were changed.

  [gbastien]
- Added `Copy groups` dashboard column.
  [gbastien]
- Make more values available in context of TAL expressions.
  Now values available in TAL expressions and in POD templates expressions
  are the same.
  [gbastien]
- Added parameter `MeetingConfig.annexEditorMayInsertBarcode` to let an annex
  editor, in addition to the `MeetingManagers`, insert a barcode into an annex.
  [gbastien]
- Added `fplog` message when using `@@reorder-items` on a meeting.
  Original order of items is also logged for examination.
  [gbastien]
- Fixed CSS for meeting select box, sometimes selecting a value
  would not click on the link and load the meeting.
  [gbastien]
- Fixed `Criteria.compute_criteria`, do not change a value of an
  existing criterion as it is actually the stored data.
  Enabled caching for `Criteria.compute_criteria`.
  [gbastien]

#### Products.MeetingCommunes (4.2.3 → 4.2.5)

#### Version 4.2.5 (2023-10-27)

- Call `PloneMeeting` migration to `4210` in MC migration to `4200`.
  [gbastien]

#### Version 4.2.4 (2023-09-12)

- Updated `attendance-stats.ods`.
  [gbastien]
- Fixed `CustomMeetingConfig.getUsedFinanceGroupIds` to work when an item has
  both inheritated and not inheritated advices, it was using the wrong
  `MeetingConfig` in some cases.
  [gbastien]
- Call `PloneMeeting` migration to `4208` in MC migration to `4200`.
  [gbastien]
- Call `PloneMeeting` migration to `4209` in MC migration to `4200`.
  [gbastien]
- Adapted `examples_fr` import_data as `MeetingConfig.useCopies` was removed.
  [gbastien]

#### imio.actionspanel (1.62 → 1.64)

#### Version 1.64 (2023-10-27)

- Fixed profile version displayed in `portal_setup` by adding a step that
  reinstalls `imio.actionspanel`.
  [gbastien]

#### Version 1.63 (2023-08-24)

- Use `uid_catalog` if available for delete by uid view [SUP-31827]
  [mpeeters]

#### imio.annex (2.18 → 2.20)

#### Version 2.20 (2023-09-04)

- Fixed conversion status update that was not working when using async conversion
  with `collective.documentviewer`.
  [gbastien]
- Display action `View preview` when a preview is available.
  [gbastien]

#### Version 2.19 (2023-08-24)

- Adapted code to new parameter `Category.show_preview`
  in `collective.iconifiedcategory`.
  [gbastien]

#### imio.helpers (0.72 → 0.77)

#### Version 0.77 (2023-10-19)

- Added `xhtml.unescape_html` that will decode HTML entities of a HTML text.
  [gbastien]

#### Version 0.76 (2023-09-28)

- Added `transmogrifier.get_correct_id` to generate a unexisting id with numbered or lettered suffix.
  [sgeulette]
- Renamed `transmogrifier.correct_path` to `transmogrifier.get_correct_path`
  [sgeulette]

#### Version 0.75 (2023-09-04)

- Fixed `setup.load_type_from_package` when loading a Dexterity FTI because
  it fails to purge old values.
  Purging is disabled for `Dexterity FTI`, added new parameter `purge_actions=False`
  that will remove the actions for a `Dexterity FTI` so it is reloaded in correct order.
  [gbastien]
- Improved `transmogrifier.str_to_date` with min and max
  [sgeulette]
- Fixed `ValueError: 'value' is not in list` in `content.sort_on_vocab_order`
  when a value of given `p_values` does not exist in the given `p_vocab`.
  [gbastien]

#### Version 0.74 (2023-08-24)

- Fixed `cache.obj_modified` when checking annotations, take care that `_p_mtime`
  is not changed on `__annotations__` when a value changes in a stored annotation
  that is a `PersistentMapping`.
  Also removed parameter `asstring=False`, when `asdatetime=False`, returned
  value is float which is convenient to be used in a cachekey.
  [gbastien]
- Add `catalog` parameter on `content.uuidsToObjects`, `content.uuidsToObject`,
  `content.uuidsToCatalogBrains` and `uuidsToCatalogBrain` to allow query on
  other catalogs (e.g. uid_catalog)
  [mpeeters]

#### Version 0.73 (2023-07-20)

- Be more defensive in `content.get_user_fullname`, in some case, a userid
  is found in `mutable_properties` but there is no properties associated with it.
  [gbastien]
- Improved `transmogrifier.clean_value` giving a replacement value
  [sgeulette]

#### imio.history (1.29 → 1.30)

#### Version 1.30 (2023-09-21)

- Added `utils.get_event_by_time` that will return an history event based
  on a given float event time.
  [gbastien]
- Formalized use of `EventPreviewView.may_view_historized_data`.
  [gbastien]

#### imio.prettylink (1.20 → 1.21)

#### Version 1.21 (2023-08-24)

- Adapted call to `imio.helpers.cache.obj_modified` as parameter `asstring=False`
  was removed, we just use the default result type that is `float`.
  [gbastien]

#### imio.pyutils (0.29 → 0.31)

#### Version 0.31 (2023-09-26)

- Added `utils.listify` that will make sure a given value
  is always returned as list-like iterable.
  [gbastien]
- Improved `system.get_git_tag` with new parameter to get last tag from all branches
  [sgeulette]
- Added `utils.radix_like_starting_1` to get list of positional numbers following a given base but starting with 1
  [sgeulette]
- Added `utils.letters_sequence` to get a letters string corresponding to nth position
  [sgeulette]

#### Version 0.30 (2023-07-24)

- Added `system.read_recursive_dir` to get files recursively (with relative or full name).
  [sgeulette]

#### imio.restapi (1.0b2 → 1.0b3)

*No changelog entries found.*

#### collective.contact.plonegroup (1.46 → 1.47)

#### Version 1.47 (2023-10-19)

- Fixed typo in french translation.
  [gbastien]

#### collective.dms.scanbehavior (1.1 → 1.3)

#### Version 1.3.0 (2023-09-07)

- Improved date range.
  [sgeulette]
- Cleanup: isort, use `unittest` instead `unittest2`,
  removed dependency on `ecreall.helpers.testing`.
  [gbastien]

#### Version 1.2 (2023-07-20)

- fix : [DMS-949] min & max for scan_date
  [bleybaert]

#### collective.eeafaceted.batchactions (1.13 → 1.14)

#### Version 1.14 (2023-09-04)

- In `BaseARUOBatchActionForm._apply`, return the elements that were actually
  updated so it may be used when overriding the base view.
  [gbastien]
- Avoided exception when a field value is None and we want to get a list or set
  [sgeulette]

#### collective.eeafaceted.collectionwidget (1.14 → 1.16)

#### Version 1.16 (2023-07-27)

- Use default value if available and if there is no parameter in request
  [mpeeters]
- Fix for Python 3 compatibilty
  [mpeeters]

#### Version 1.15 (2023-07-03)

- Ensure that parent can be displayed if `hide_category` is True and without category
  [mpeeters]
- Add `hide_category` option (False by default) to add the possibility to hide category titles
  [mpeeters]

#### collective.eeafaceted.z3ctable (2.21 → 2.25)

#### Version 2.25 (2023-10-27)

- In `DateColumn.renderCell`, no need to manage a `DateTime` as it is supported
  by `api.portal.get_localized_time`.
  [gbastien]

#### Version 2.24 (2023-10-19)

- Added `PrettyLinkWithAdditionalInfosColumn.ai_reloaded_fields` functionnality:
  this will force update cached widget and remove its terms if any, this is
  useful when using a context aware vocabulary.
  [gbastien]
- Removed the `PrettyLinkWithAdditionalInfosColumn` `get_ai_xxx` accessors,
  access the attribute directly instead.
  [gbastien]
- Added attribute `BaseColumn.the_object=False`, this means that we are getting
  the information on the object and not on the brain.
  Removed recently added columns `AwakeObjectVocabularyColumn` and
  `AwakeObjectAbbrColumn`, simply use `the_object=True` in this case.
  [gbastien]

#### Version 2.23 (2023-09-04)

- Added `AwakeObjectVocabularyColumn` and `AwakeObjectAbbrColumn`, having same
  behavior as `VocabularyColumn` and `AbbrColumn` but `attrName` is get on awaken
  object instead brain metadata, this avoids adding a `portal_catalog` metadata.
  [gbastien]
- In `AwakeObject` columns, use `imio.helpers.content.base_getattr` instead
  `getattr` to avoid problems with acquisiton.
  [gbastien]

#### Version 2.22 (2023-08-24)

- Rely on `imio.helpers.content.get_user_fullname` that manages fallback to
  `getMemberInfo` if fullname not found in `mutable_properties`.
  This needs to rely on `imio.helpers` that is now a dependency.
  [gbastien]

#### collective.iconifiedcategory (0.57 → 0.60)

#### Version 0.60 (2023-09-21)

- Fixed version (2105) in `metadata.xml`.
  [gbastien]

#### Version 0.59 (2023-09-04)

- Display the document conversion spinner in any relevant case.
  [gbastien]
- Added `contentType` value to the `categorized_elements` data.
  [gbastien]

#### Version 0.58 (2023-08-24)

- Added new field `ICategorize.show_preview` to turn link to element to a
  `collective.documentviewer` preview instead download.
  Fixed icon displayed when preview computation in progress.
  [gbastien]
- Force icon `width/height` to `16px` in `tooltipster`
  (`categorized-childs.pt` and `categorized-childs-infos.pt`).
  [gbastien]
- Fixed `ContentCategory` portal_type title in `ContentCategory.xml`.
  [gbastien]

#### collective.messagesviewlet (1.0b2 → 1.0b3)

*No changelog entries found.*

#### imio.pm.locales (4.2.4 → 4.2.8)

#### Version 4.2.8 (2023-10-27)

- Added translation for new advice type `Read`.
  [gbastien]
- Added translation for advice behavior `title_advice_accounting_commitment`.
  [gbastien]
- Added translation for `label_advice_given_by`.
  [gbastien]

#### Version 4.2.7 (2023-10-19)

- Adapted translations as now we do not use brackets to manage optional advisers
  but label `[auto]` for automatically asked advices.
  [gbastien]
- Added translations for new field `MeetingItem.meetingDeadlineDate` and
  related faceted dashboard column.
  [gbastien]
- Added translations for new advice types `negative_with_remarks` and
  `back_to_proposing_group`.
  [gbastien]

#### Version 4.2.6 (2023-09-21)

- Added translation for `Item completeness changed`.
  [gbastien]

#### Version 4.2.5 (2023-09-12)

- Adapted translations regarding `ContentCategory` refactoring and possibility
  to not keep an annex when item sent to other MC.
  [gbastien]
- Adapted `other_mc_correspondences_descr` regarding last changes.
  [gbastien]
- Added translations for new `Copy groups` column and `Change copy groups` batch action.
  [gbastien]
- Removed translations for `MeetingConfig.useCopies` as field was removed.
  [gbastien]
- Added translations for `MeetingConfig.annexEditorMayInsertBarcode`.
  [gbastien]

#### imio.pm.ws (3.7 → 3.8)

#### Version 3.8 (2023-10-19)

- Make sure `createItemRequest` returns a response status of `200` or
  it raises a `SOAPException` (even if item is created anyway?!).
  [gbastien]
- Fixed `SOAPView._getItemInfos` when computing `preferred_meeting_date`, it was
  always `None` because using the `uid_catalog` and Meeting is a DX content type.
  [gbastien]

#### imio.zamqp.pm (0.16 → 0.18)

#### Version 0.18 (2023-10-27)

- Removed `config.BARCODE_INSERTED_ATTR_ID`, we do not use it anymore to check
  if a barcode was inserted, we rely on the `scan_id`.
  [gbastien]

#### Version 0.17 (2023-09-04)

- Moved `collective.iconifiedcategory` `ContentCategory` overrides
  back to `Products.PloneMeeting`.
  [gbastien]
- Cleaned code:

  - removed event that deleted copied annexes with a `scan_id`,
    now managed by `Products.PloneMeeting`;
  - removed setup for `scan_id` index, done by `collective.dms.scanbehavior`.

  [gbastien]
- Take into account new parameter `MeetingConfig.annexEditorMayInsertBarcode`
  in `InsertBarcodeView.may_insert_barcode`.
  [gbastien]

#### plonemeeting.restapi (2.1 → 2.2)

#### Version 2.2 (2023-09-12)

- Always include `@type` info in result even when `include_base_data=false` as
  it is used with `UidSearchGet.required_meta_type_id`.
  [gbastien]

#### plonetheme.imioapps (2.42 → 2.43)

#### Version 2.43 (2023-08-24)

- Fix document generation actions on dashboard for urban [URB-2863]
  [mpeeters]
- Fix faceted autocomplete widget width in urban [URB-2866]
  [jchandelle]
- Removed styling rule for `.tooltipster-base img` as image `height/width`
  is now forced to `16px` in `collective.iconifiedcategory`.
  [gbastien]

## Release 4.2.20

**Date:** 2023-08-31

### Package Updates

#### Products.PloneMeeting (4.2.2 → 4.2.4)

#### Version 4.2.4 (2023-07-12)

- Added batch action to change groups in charge.
  Moved batchactions to `bacthactions.py`.
  [gbastien]
- Added faceted filter `Creator` (enabled by default) on listings of meetings.
  [gbastien]
- Added upgrade step to re-enable fields `meeting.videoconference` and
  `meeting.extraordinary_session` if it was used on a previous meeting.
  [gbastien]

#### Version 4.2.3 (2023-07-07)

- Fixed `lateItem` item mail notification that was broken because still using
  the `uid_catalog` and meeting DX does not use it anymore.
  [gbastien]
- Completed meeting categories functionality:

  - Added optional column in dashboards displaying meetings;
  - Added faceted filter in dashboards displaying meetings
    (this rely on new parameter `MeetingConfig.dashboardMeetingsListingsFilters`).

  [gbastien]
- Added `imio.helpers.workflow.update_role_mappings_for` to `safe_utils`.
  [gbastien]
- Added `itemdecided` workflow adaptation that will add a state `itemdecided` in
  the item workflow between `itempublished` and `accepted`.
  [gbastien]
- Keep field `MeetingItem.isAcceptableOutOfMeeting` when item duplicated in the
  same MC (or from an item template).
  `isAcceptableOutOfMeeting` is set back to `False` when using workflow adaptations
  `accepted_out_of_meeting_and_duplicated` and
  `accepted_out_of_meeting_emergency_and_duplicated` as item is duplicated to be
  presented in a next meeting.
  [gbastien]
- `get_state_infos` was moved from `imio.helpers.content` to
  `imio.helpers.workflow`, adapted import accordingly.
  [gbastien]
- Replaced `MeetingItemWorkflowActions._latePresentedItem` by
  `MeetingItemWorkflowActions._latePresentedItemTransitions` that just needs
  a tuple of transitions to trigger on a late item, easier to override.
  [gbastien]
- Updated link to the documentation.
  [gbastien]

#### Products.MeetingCommunes (4.2.2 → 4.2.3)

#### Version 4.2.3 (2023-07-07)

- Removed confusing `transition_done_descr` translations
  (portal message displayed after a transition).
  [gbastien]
- Added translations for `create_to_bourgmestre_from_meeting-config-college`
  and `create_to_bourgmestre_from_meeting-config-college_comments`.
  [gbastien]
- Updated link to the documentation.
  [gbastien]

#### imio.dashboard (2.10 → 2.12)

#### Version 2.12 (2023-07-07)

- `get_transitions` was moved from `imio.helpers.content` to `imio.helpers.workflow`.
  [gbastien]

#### Version 2.11 (2023-03-22)

- Changes for WCA compatibility.
  [odelaere]

#### imio.helpers (0.70 → 0.72)

#### Version 0.72 (2023-07-12)

- In `submitFormHelperOnsuccessDefault` JS function, only manage `blob` if
  `content-type` is `application/xxx`.
  [gbastien]
- Added `content.sort_on_vocab_order` that will sort a list of `values`
  respecting a given `vocabulary` terms order. This relies on `sort_by_indexes`
  from `imio.pyutils` that is now a dependency.
  [gbastien]

#### Version 0.71 (2023-07-07)

- Modified `transmogrifier.relative_path` to add option to keep leading slash
  (True by default).
  [sgeulette]
- In `content.get_user_fullname`, if `fullname` not found at the end,
  finally fallback to `portal_membership.getMemberInfo`, this is sometimes
  necessary when using LDAP.
  [gbastien]
- Removed backward compatible imports for `get_state_infos`, `get_transitions`
  and `do_transitions` moved from `content` to `workflow`.
  [gbastien]

#### collective.contact.plonegroup (1.45 → 1.46)

#### Version 1.46 (2023-07-07)

- Added parameter `omitted_suffixes=[]` to `utils.get_all_suffixes`.
  [gbastien]

#### collective.eeafaceted.batchactions (1.12 → 1.13)

#### Version 1.13 (2023-07-12)

- Added `BaseARUOBatchActionForm`, a class factorizing the action that
  `add/remove/update/overwrite` values on an attribute of an object
  (originally used for the `LabelsBatchActionForm`) so it is easier to reuse
  for other similar actions. `LabelsBatchActionForm` is now based on that
  `BaseARUOBatchActionForm`.
  [gbastien]
- Activated `delete-batch-action` for zope admin
  [sgeulette]

#### imio.pm.locales (4.2.2 → 4.2.4)

#### Version 4.2.4 (2023-07-12)

- Removed unused translation `groups_in_charge_can_not_be_empty_batch_action_warning`,
  is managed by `collective.eeafaceted.batchations` now.
  [gbastien]

#### Version 4.2.3 (2023-07-07)

- Completed translations related to the `meeting.category` functionality.
  [gbastien]
- Added translations related to the `itemdecided` workflow adaptation.
  [gbastien]
- Added translations related to the `Update groups in charge` batch action.
  [gbastien]

#### plonetheme.imioapps (2.41 → 2.42)

#### Version 2.42 (2023-07-07)

- `get_state_infos` was moved from `imio.helpers.content` to
  `imio.helpers.workflow`, adapted import accordingly.
  [gbastien]

## Release 4.2.19

**Date:** 2023-07-04

### Package Updates

#### Products.PloneMeeting (4.2.1 → 4.2.2)

#### Version 4.2.2 (2023-06-27)

- Fixed `MeetingConfig.validate_workflowAdaptations`. Removing a `waiting_advices`
  complementary configuration is allowed, only check for items in review_state
  `waiting_advices` if the `waiting_advices` WFA was removed.
  [gbastien]
- Set `MeetingStoreItemsPodTemplateAsAnnexBatchActionForm.available_permission`
  to `ManagePortal`, this new feature from `collective.eeafaceted.batchactions`
  avoids overriding the `available` method.
  [gbastien]
- Fixed `Migrator.updateWFStatesAndTransitions` that was broken now that
  `MeetingConfig STATE_ATTRS/TRANSITION_ATTRS` manage `DataGridFields`.
  [gbastien]
- `check_zope_admin` was moved from `Products.CPUtils` to `imio.helpers.security`.
  [gbastien]
- Make sure tables with no border are dispalyed as this in every cases
  (view, dashboards, CKEditor, ...).
  [gbastien]
- Adapted `BatchActions` to use new attribute `available_permission` to avoid
  overriding the `available` method.
  [gbastien]
- Added `category` on meetings.
  [gbastien]
- Fixed reference not displayed on item in state `presented` when using
  `MeetingConfig.computeItemReferenceForItemsOutOfMeeting`.
  [gbastien]
- In users management, a real Zope admin may remove a user.
  [gbastien]
- Pass `mimetype='text/plain'` in `renderComments` methods to avoid
  `portal_transforms` wrong `mimetype` detection.
  [gbastien]
- Fixed `SelectableCommitteesVocabulary`, make sure if a value is stored,
  it is always in the vocabulary no matter it has `usingGroups`.
  [gbastien]
- When using `MeetingConfig.usingGroups`, make sure we do not let the role
  `MeetingObserverGlobal` access the meetings or groups that are not in
  `MeetingConfig.usingGroups` have access and also receive mail notifications
  about meeting events.
  Because of code order (events are called before the
  `at_post_create_script/at_post_edit_script`), all this was cleaned, we do
  no more use the `at_post_create_script/at_post_edit_script`.
  [gbastien]

#### Products.MeetingCommunes (4.2.1 → 4.2.2)

#### Version 4.2.2 (2023-06-27)

- Call PloneMeeting migrations to 4206 and 4207 in MC migration to 4200.
  [gbastien]

#### imio.helpers (0.69 → 0.70)

#### Version 0.70 (2023-06-21)

- Added `security.check_zope_admin` (moved from `Products.CPUtils`).
  [gbastien]
- Improved `transmogrifier.filter_keys`
  [sgeulette]
- Added `workflow.update_role_mappings_for` helper to update WF role mappings
  for a given object.
  [gbastien]

#### imio.history (1.28 → 1.29)

#### Version 1.29 (2023-06-27)

- Make `IHContentHistoryView.renderComments` more robust by passing original
  `mimetype='text/plain'` to avoid `portal_transforms` detecting it automatically
  that can lead to wrong detection.
  [gbastien]

#### imio.pyutils (0.27 → 0.29)

#### Version 0.29 (2023-05-12)

- Improved `utils.all_of_dict_values` to include optionally a label.
  [sgeulette]
- Added `setup_logger` to modify a given logger independently
  [sgeulette]
- Added `full_path` to prefix filename with path if necessary
  [sgeulette]

#### Version 0.28 (2023-03-29)

- Added `utils.one_of_dict_values` that gives the first non empty value of a list of keys.
  [sgeulette]
- Added `utils.all_of_dict_values` that returns a not empty values list from a dict following a keys list
  [sgeulette]

#### collective.behavior.talcondition (0.14 → 1.0a1)

#### Version 1.0.0 (2024-09-18)

- Generated universal wheel version.
  [sgeulette]

#### Version 1.0a2 (2024-09-16)

- Fix dict iteration for Python 3
  [laulaz]
- Updated Makefile
  [sgeulette]
- Used pyenv in gha
  [sgeulette]

#### Version 1.0a1 (2023-06-21)

- Fix deprecated import AccessControl.class_init instead of App.class_init
  (Plone6 compatibility)
  [boulch]
- Set simplier setup with Makefile
  [sgeulette]

#### collective.documentgenerator (3.38 → 3.39)

#### Version 3.39 (2023-06-26)

- Removed `utils.safe_encode`, imported it from `imio.helpers.content`.
  [gbastien]

#### collective.eeafaceted.batchactions (1.11 → 1.12)

#### Version 1.12 (2023-06-27)

- Added action to `Update WF role mappings`.
  Moved `available_permission` functionality from `ContactBaseBatchActionForm`
  to `BaseBatchActionForm` so it is available for any action.
  Added `BaseBatchActionForm.available_for_zope_admin` that makes an action
  only available to the Zope admin.
  [gbastien]
- Make `UpdateWFRoleMappingsActionForm` use
  `imio.helpers.workflow.update_role_mappings_for`.
  [gbastien]

#### collective.eeafaceted.z3ctable (2.19 → 2.21)

#### Version 2.21 (2023-06-27)

- In `PrettyLinkWithAdditionalInfosColumn`, in the cached view, update widget
  when it is a `RelationChoice/RelationList` to get correct value.
  [gbastien]

#### Version 2.20 (2023-06-21)

- Corrected iteration problem if gotten value for column is None.
  [sgeulette]

#### imio.pm.locales (4.2.1 → 4.2.2)

#### Version 4.2.2 (2023-06-27)

- Removed unused translations `show_or_hide_pollTypeObservations` and `Toggle descriptions of items`.
  [gbastien]
- Added translations for `meeting.category` related functionality.
  [gbastien]
- Reworked `advice_given_or_modified` french translation so it is more clear to the user.
  [gbastien]
- Make french translation for `wa_only_creator_may_delete` more accurate.
  [gbastien]
- Added translations related to `meeting_remove_global_access` WFA.
  [gbastien]

#### plonemeeting.restapi (2.0.2 → 2.1)

#### Version 2.1 (2023-06-27)

- In `base.serialize_attendees`, do not use `UID` from serialized result as it
  could not be there when using `include_base_data=false`.
  [gbastien]

#### plonetheme.imioapps (2.39 → 2.41)

#### Version 2.41 (2023-06-27)

- Style table header the same way for HTML tables and DX/AT datagrid fields.
  [gbastien]

#### Version 2.40 (2023-06-15)

- Add a red color to the denied status of divisions
  [fngaha]

#### Products.CPUtils (1.22 → 1.23)

#### Version 1.23 (2023-06-26)

- Added parameter `use_registry=False` to `configure_ckeditor`, set it to `True`
  with `collective.ckeditor 4.11+`.
  [gbastien]
- Removed file `CONTRIBUTORS.rst`.
  [gbastien]
- `utils.check_zope_admin` has been moved to `imio.helpers.security`.
  [gbastien]
- Removed `utils.safe_encode` as already imported from `imio.helpers.content`.
  [gbastien]

## Release 4.2.18

**Date:** 2023-06-08

### Package Updates

#### Products.PloneMeeting (4.2 → 4.2.1)

#### Version 4.2.1 (2023-05-31)

- Do no more use `ToolPloneMeeting.get_plone_groups_for_user`,
  use `imio.helpers.cache.get_plone_groups_for_user` instead.
  [gbastien]
- Added `fingerpointing-like` log when sending an email.
  [gbastien]
- Fixed `PersonalLabelsAdapter` that breaks if no labels selected in query index.
  [gbastien]
- Fixed disabled attendees styling in meeting edit form.
  [gbastien]
- Changed position of `photo` and `signature` fields on `person`,
  moved `signature` before `photo`.
  [gbastien]
- Adapted code to manage attendees thru `restapi` `@attendee/@attendees`
  endpoints on meeting and item.
  Added possibility to edit a redefined item signatory.
  [gbastien]
- Fixed `PMDataChangesHistoryAdapter` when historizing multivalued fields
  (`MeetingItem.copyGroups` for example) and some old values are no more in
  existing values.
  [gbastien]
- Removed JS alert `hello` when ajax saving rich text.
  [gbastien]
- Make `is_all_count` available again on the `ItemDocumentGenerationHelperView`.
  It was moved out together with `print_votes`.
  [gbastien]
- Fixed item advices invalidation, advices were removed but not unindexed.
  In `Migrate_To_4205._initAdviceGivenHistory`, call `clean_catalog_orphans` to
  clean potential `meetingadvice` orphan when using
  `MeetingConfig.enableAdviceInvalidation`.
  [gbastien]
- Reordered fields on `MeetingConfig`, moved `xhtmlTransformTypes` just under
  `xhtmlTransformFields`.
  [gbastien]
- Make sure annex are not kept upon duplication (to same or distant MC)
  if annex type requires a PDF file and the annex file is not PDF.
  [gbastien]
- Fixed action `Delete whole meeting` when triggered from dashboards, was
  redirecting resulting in a broken dashboard because collection `UID` was lost.
  [gbastien]
- Adapted `MeetingItem.setPreferredMeeting` and `MeetingItem._update_preferred_meeting`
  to manage empty or wrong value when creating an item using `restapi`.
  [gbastien]
- Fixed `PMExistingPODTemplate`, do not break if the reusable `PODTemplate` is not
  stored in the `podtemplates` folder of a `MeetingConfig`, it could be in the
  `contacts` directory or somewhere else.
  [gbastien]
- Make sure transitions are rendered in the actions_panel displayed on advices.
  This is necessary for cases were a complex workflow is used for advices.
  [gbastien]
- Completed `MeetingConfig.validate_workflowAdaptations` and
  `MeetingConfig.validate_itemWFValidationLevels` to factorize translations and
  check transitions and states used in datagridfields.
  [gbastien]
- Fixed translation of `Data that will be used on new item` on `meetingitem_view.pt`.
  [gbastien]
- Make sure `MeetingItem.getCategory` and `MeetingItem.getClassifier` do not break
  when attribute is `None`, this may happen when item created by REST WS and
  `catefory/classifier` validation is disabled.
  [gbastien]
- On tool view, display also configs that are not active (in red).
  [gbastien]
- Make sure `MeetingItem.otherMeetingConfigsClonableToFieldXXX` fields are
  displayed in Schema defined order on the item edit and view.
  [gbastien]
- Added possibility to have an incremental internal number for items.
  This relies on `collective.behavior.internalnumber`.
  [gbastien]
- Moved `monkey._listAllowedRolesAndUsers` to
  `imio.helpers.patches._listAllowedRolesAndUsers`.
  [gbastien]

#### Products.MeetingCommunes (4.2 → 4.2.1)

#### Version 4.2.1 (2023-05-31)

- Fixed `zbougmestre` profile `shortName` from wrong `AG` to `Bourgmestre`.
  [gbastien]

#### appy (1.0.14 → 1.0.15)

*No changelog entries found.*

#### imio.helpers (0.66 → 0.69)

#### Version 0.69 (2023-05-31)

- Monkeypatch `CatalogTool._listAllowedRolesAndUsers` to add `ram.cache` decorator.
  [gbastien]

#### Version 0.68 (2023-05-12)

- Added `split_text` in transmogrifier module.
  [sgeulette]
- Added `workflow.get_leading_transitions` that will return every WF transitions
  leading to a given `state_id`.
  [gbastien]

#### Version 0.67 (2023-03-29)

- Added `clean_value`, `correct_path`, `filter_keys`, `get_obj_from_path` in transmogrifier module.
  [sgeulette]
- Added `key_val`, `pool_tuples`, `str_to_date` in transmogrifier module.
  [sgeulette]
- Renamed `text_int_to_bool` to `str_to_bool`
  [sgeulette]

#### imio.migrator (1.32 → 1.33)

#### Version 1.33 (2023-04-14)

- Added `Migrator.clean_orphan_brains` that will uncatalog orphan brains.
  [gbastien]

#### imio.restapi (1.0b1 → 1.0b2)

*No changelog entries found.*

#### collective.compoundcriterion (0.6 → 0.7)

#### Version 0.7 (2023-04-12)

- Do not break in `negative-previous-index` when some filters does not have
  values (so the `'v'` is not there in the query).
  [gbastien]

#### imio.pm.locales (4.2 → 4.2.1)

#### Version 4.2.1 (2023-05-31)

- Adapted translations regarding `@attendees` restapi endpoints.
  [gbastien]
- Renamed translations `item_not_present_type_absent`/`item_not_present_type_excused`/
  `item_not_present_type_non_attendee` by `absent/excused/non_attendee` so it is
  easier to reuse in other contexts.
  [gbastien]
- Added translation for `annex_not_kept_because_only_pdf_annex_type_warning`.
  [gbastien]
- Refactored translations related to `MeetingConfig.validate_workflowAdaptations`
  and `MeetingConfig.validate_itemWFValidationLevels` now that states/transitions
  are checked in datagridfields.
  [gbastien]
- Completed `max_shown_...` translations to add warning about selecting a too high value.
  [gbastien]
- Fixed some typos in french translations.
  [gbastien]
- Adpated translation of `compute_item_reference_for_items_out_of_meeting_descr`
  to specify that it will update item reference of items out of meeting.
  [gbastien]

#### plone.restapi (7.8.0 → 7.8.2)

*No changelog entries found.*

#### plonemeeting.restapi (2.0.1 → 2.0.2)

#### Version 2.0.2 (2023-05-31)

- Added `@attendees GET` on meeting and item and `@attendee GET/PATCH`
  on meeting and item. Added `extra_include=attendees` on meeting and item.
  [gbastien]
- Manage `metadata_fields=internal_number`.
  [gbastien]

#### plonetheme.imioapps (2.38 → 2.39)

#### Version 2.39 (2023-03-29)

- Fixed css to align multi select2 widget to the left.
  [sgeulette]

## Release 4.2.17

**Date:** 2023-05-24

### Package Updates

#### Products.PloneMeeting (4.2rc34 → 4.2)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b24 → 4.2)

*No changelog entries found.*

#### appy (1.0.12 → 1.0.14)

*No changelog entries found.*

#### imio.actionspanel (1.60 → 1.62)

#### Version 1.62 (2023-02-27)

- Fixed rendering of error message when an exception occurs during a transition.
  [gbastien]
- Added new action `renderOwnDeleteWithComments=False` when deleting an element
  a comment may be entered, the deletion including comment will appear in the
  history of the parent of the element that was deleted.
  [gbastien]
- In JS function `deleteElement`, call event `ap_delete_givenuid` also when
  parameter `redirect=0`.
  [gbastien]

#### Version 1.61 (2022-10-14)

- Force by default redirect after transition just when use icons
  [fngaha]

#### imio.dashboard (2.9 → 2.10)

#### Version 2.10 (2022-10-25)

- Adapts generationlink viewlet to last `collective.documentgenerator` last changes.
  [sdelcourt]

#### imio.helpers (0.62 → 0.66)

#### Version 0.66 (2023-02-13)

- Added `transmogrifier` module with `get_main_path`, `relative_path` and
  `text_int_to_bool` functions.
  [sgeulette]
- Added `none_if_unfound` parameter in `get_user_fullname` function
  [sgeulette]
- Added parameter `onsuccess=false` to JS function `callViewAndReload` so it is
  possible to trigger custom JS code after a success.
  [gbastien]
- Added `xhtml.is_html` that will return True or False if given text is HTML or not.
  [gbastien]
- Raised validation error when email realname contains an accented character
  [sgeulette]

#### Version 0.65 (2022-12-07)

- Return new date when `cache.invalidate_cachekey_volatile_for` is called with
  `get_again=True`.
  [gbastien]
- Use `dict.items` instead `dict.iteritems` for Py2/Py3 compatibility.
  [gbastien]

#### Version 0.64 (2022-10-28)

- Added `workflow.remove_state_transitions` function do remove transitions on a state and clean duplicates
  [sgeulette]
- Added more tests on cached methods.
  [sgeulette]

#### Version 0.63 (2022-09-01)

- Invalidated '_users_groups_value' volatile after a call of `GroupAwareRoleManager.assignRolesToPrincipal`,
  `ZODBRoleManager.assignRoleToPrincipal` and `ZODBRoleManager.removeRoleFromPrincipal`
  [sgeulette]
- Removed duplicated classifiers.
  [sgeulette]

#### imio.history (1.27 → 1.28)

#### Version 1.28 (2023-02-27)

- Added possibility to display an event preview under the comment
  in the `@@contenthistory` view.
  [gbastien]
- Make the `highlight_last_comment` functionnality generic, it was only used
  with WF history but now any history may be set `highlight_last_comment=True`.
  [gbastien]

#### imio.pyutils (0.25 → 0.27)

#### Version 0.27 (2023-02-27)

- Added `utils.sort_by_indexes` that will sort a list of values
  depending on a list of indexes.
  [gbastien]

#### Version 0.26 (2022-12-12)

- Added `stop` to print error and exit.
  [sgeulette]

#### collective.compoundcriterion (0.5 → 0.6)

#### Version 0.6 (2023-02-13)

- Added `negative-previous-index` and `negative-personal-labels` default adapters.
  Rely on `imio.helpers`. Removed dependency on `unittest2`.
  [gbastien]

#### collective.contact.plonegroup (1.44 → 1.45)

#### Version 1.45 (2023-02-27)

- Avoid useless variable initialization in `utils.get_plone_group`,
  do everything in one line.
  [gbastien]

#### collective.documentgenerator (3.35 → 3.38)

#### Version 3.38 (2022-12-12)

- Added missing upgrade step after registry modification (`force_default_page_style_for_mailing`) in 3.36.
  [sgeulette]

#### Version 3.37 (2022-10-27)

- Bugfix: page style check now handle case of POD template without mailing template
  attribute.
  [sdelcourt]

#### Version 3.36 (2022-10-21)

- Add a new parameter `force_default_page_style_for_mailing` to the registry.
  If set to True, apply automatically a default page style to mailing templates.
  [sdelcourt]
- Order templates directories by title in `dg-templates-listing` view.
  [sgeulette]
- Improved `DXDocumentGenerationHelperView.get_value` by adding optional obj parameter.
  [sgeulette]

#### collective.eeafaceted.z3ctable (2.18 → 2.19)

#### Version 2.19 (2023-02-27)

- Extended JS function `toggleCheckboxes` to pass the select/unselect checkbox
  as first parameter and trigger the click event when checkboxes checked or unchecked.
  This changes nothing here but makes this function more useable in other contexts.
  [gbastien]
- JS function `preventDefaultClickTransition` was renamed to
  `preventDefaultClick` in `imio.actionspanel>=1.62`.
  [gbastien]
- Do not break in `I18nColumn` when translating a string with special chars.
  [gbastien]

#### collective.iconifiedcategory (0.55 → 0.57)

#### Version 0.57 (2023-03-30)

- When no request (when using `plone.app.async`), pass `None` instead `{}`
  to `ImageDataModifiedImageScaling` so `plone.namedfile` scaling is happy
  when using `plone.protect >= 3`.
  [aduchene]

#### Version 0.56 (2023-02-27)

- Adapted french translation for `More infos`.
  [gbastien]

#### collective.messagesviewlet (0.23 → 1.0b2)

*No changelog entries found.*

#### imio.pm.locales (4.2b31 → 4.2)

*No changelog entries found.*

#### imio.pm.ws (3.6 → 3.7)

#### Version 3.7 (2023-03-06)

- Fixed `test_ws_getItemInfosWithShowAssembly` regarding changes in default
  contacts gender in PloneMeeting testing profile `import_data`.
  [gbastien]
- Completed `test_ws_meetingAcceptingItems` to check that it works when using
  `inTheNameOf` (was actually not working before `Products.PloneMeeting==4.2rc30`).
  [gbastien]
- Adapted code regarding removal of `MeetingConfig.useGroupsAsCategories`.
  [gbastien]

#### imio.zamqp.core (0.6 → 0.7)

#### Version 0.7 (2022-10-28)

- Corrected parameter typo in `utils.next_scan_id` and `utils.scan_id_barcode`.
  Added sphinx compliant doc strings.
  [sgeulette]

#### imio.zamqp.pm (0.15 → 0.16)

#### Version 0.16 (2023-02-27)

- Adapted call to `imio.zamqp.core.utils.next_scan_id` where typo in parameter
  `cliend_id_var` was fixed to `client_id_var`.
  [gbastien]

#### plonemeeting.restapi (1.0rc18 → 2.0.1)

#### Version 2.0.1 (2023-03-07)

- Fixed test isolation problem when tests executed together with `imio.pm.ws` tests.
  [gbastien]

#### Version 2.0 (2023-03-06)

- Dropped support for `PloneMeeting 4.1.x`.
  [gbastien]
- Add `config` to `extra_include` allowed parameters to return informations about the meeting config
  [mpeeters]
- Ensure that `in_name_of` parameter is only handled once when `__children__` parameter is used
  [mpeeters]
- Enforce usage of `UID` parameter only if `externalIdentifier` is not provided
  [mpeeters]
- Added `test_restapi_add_item_manually_linked_items` to check that it is possible
  to create items and use the `MeetingItem.manuallyLinkedItems` functionnality.
  [gbastien]
- Adapted code as `MeetingConfig.useGroupsAsCategories` was removed.
  Field `MeetingItem.category` is an optional field managed by
  `MeetingConfig.usedItemAttributes` as any other optional fields now.
  [gbastien]
- Add `date` by default to meeting informations.
  [mpeeters]

#### plonetheme.imioapps (2.37 → 2.38)

#### Version 2.38 (2023-02-13)

- Added `.no-style-table tr.hide-bottom-border` that will remove
  the bottom border when displaying fields in a table.
  [gbastien]
- Avoid large image breaking the advice tooltipster.
  [gbastien]
- Style results displayed in `referencebrowserwidget`.
  [gbastien]
- Adapted override of `collective.messagesviewet` viewlet manager as base class
  and definition were changed since integration of global/local messages.
  [gbastien]
- Make `ftw.labels` configuration label edit overlay larger.
  [gbastien]

## Release 4.2.16

**Date:** 2023-02-24

### Package Updates

#### Products.PloneMeeting (4.2rc31 → 4.2rc34)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b22 → 4.2b24)

*No changelog entries found.*

#### imio.pyutils (0.24 → 0.25)

#### Version 0.25 (2022-09-16)

- Added `get_git_tag`.
  [sgeulette]

#### collective.iconifiedcategory (0.54 → 0.55)

#### Version 0.55 (2022-09-29)

- Fixed `utils.get_ordered_categories` and
  `IconifiedCategoryGroupAdapter.get_every_categories` to make sure returned
  categories are from the correct `config_root` and `cachekey` is invalidated
  if `config_root` changed.
  [gbastien]

#### imio.pm.locales (4.2b29 → 4.2b31)

*No changelog entries found.*

#### Products.CPUtils (1.21 → 1.22)

#### Version 1.22 (2022-09-19)

- Automatically install External methods at the root of Zope app.
  [odelaere]

## Release 4.2.15

**Date:** 2022-09-15

### Package Updates

#### Products.PloneMeeting (4.2rc30 → 4.2rc31)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b21 → 4.2b22)

*No changelog entries found.*

#### imio.helpers (0.61 → 0.62)

#### Version 0.62 (2022-08-19)

- Added `IMIORAMCache` using `IMIOStorage` to extend used cache duration and
  improve displayed statistics
  [gbastien]
- Added cache on various acl methods following `decorate_acl_methods` env variable
  [gbastien, sgeulette]
- Added IIMIOLayer BrowserLayer (need to execute upgrade step to 2).
  [gbastien]
- Override `caching-controlpanel-ramcache` to compute totals for `Hits`, `Misses`,
  `Size` and `Entries`, display `Older entry`, do not break to display statistics
  when a pickle error occurs but add a portal message.
  [gbastien]
- Added parameter `ttl=0` to `cache.get_cachekey_volatile` this way a date older
  than given `ttl` (in seconds) will be recomputed.
- Added 'none_if_no_user' param in `content.get_user_fullname`.
  [sgeulette]
- Always return unicode in `content.get_user_fullname`.
  [sgeulette]
- Added `test_helpers.ImioTestHelpers` class with useful methods from iA.delib
  [sgeulette]
- Added `vocabularies.SimplySortedUsers` and modified `vocabularies.SortedUsers`
  [sgeulette]
- Added `cache.get_users_in_plone_groups`
  [sgeulette]
- Added `setup.load_type_from_package` to reload a single type.
  Moved `workflow.load_workflow_from_package` to `setup.load_workflow_from_package`.
  [gbastien]

#### imio.migrator (1.31 → 1.32)

#### Version 1.32 (2022-07-01)

- Added `utils.ensure_upgraded` that will make sure a given `package_name` is upgraded,
  this is useful when some content or registry records need to be present to handle some code.
  Here the usecase is a Zope starting handler needing a registry record that may not be present
  if package not upgraded.
  [gbastien]

#### imio.pyutils (0.23 → 0.24)

#### Version 0.24 (2022-08-19)

- Added `utils.time_start` and `utils.time_elapsed` to print elapsed time from start.
  Intended to be easily used when debugging...
  [sgeulette]

#### collective.contact.plonegroup (1.43 → 1.44)

#### Version 1.44 (2022-08-19)

- Warning, changed behavior of `utils.get_organization`, added parameter
  `only_in_own_org=True` that will make sure that given `org_uid` is an
  organization inside own organization.
  [gbastien ]
- Added `get_selected_org_suffix_principal_ids` and `voc_selected_org_suffix_userids`
  to work only with group and user ids
  [sgeulette]
- Used cached method `get_users_in_plone_groups` from imio.helpers
  [sgeulette]

#### collective.documentgenerator (3.34 → 3.35)

#### Version 3.35 (2022-08-26)

- Group link by template title.
  [odelaere]
- Added 'title' attribute to generation link.
  [odelaere]
- Aliased import to avoid confusion.
  [sgeulette]
- CSS for generationlinks so it may be adapted more easily.
  [gbastien]

#### collective.eeafaceted.dashboard (0.19 → 0.20)

#### Version 0.20 (2022-08-26)

- Adapted `DashboardDocumentGeneratorLinksViewlet.get_links_info` to be
  compatible with `collective.documentgenerator>=3.35`.
  [gbastien]

#### imio.pm.locales (4.2b28 → 4.2b29)

*No changelog entries found.*

#### plonemeeting.restapi (1.0rc17 → 1.0rc18)

*No changelog entries found.*

#### plonetheme.imioapps (2.36 → 2.37)

#### Version 2.37 (2022-08-26)

- CSS for `generationlinks` from `collective.documentgenerator` now that templates
  are grouped by title, the title is no more clickable so make the icon larger,
  make the icons look like buttons.
  [gbastien]
- On hover of `prettylink` in `#portal-column-one`, apply same styles as in `#content`.
  [gbastien]
- Removed rule `vertical-align: bottom;` for `#content input`.
  [gbastien]
- Fixed contenttype icon `max-width` to 16px, necessary when the img is a svg.
  [gbastien]

## Release 4.2.14

**Date:** 2022-08-26

### Package Updates

#### Products.PloneMeeting (4.2rc29 → 4.2rc30)

*No changelog entries found.*

#### imio.helpers (0.58 → 0.61)

#### Version 0.61 (2022-07-01)

- Moved workflow related functions from content to workflow module.
  [sgeulette]
- Added `workflow.load_workflow_from_package` to reload a single workflow.
  [sgeulette]
- Be defensive in JS function `toggleDetails` if tag is not available.
  [gbastien]

#### Version 0.60 (2022-06-24)

- Handled unfound site in `set_site_from_package_config`.
  [sgeulette]

#### Version 0.59 (2022-06-21)

- Added `escaped=True` param on `xhtml.object_link`.
  [sgeulette]
- Require a version of `future` recent enough so `html.escape` is available.
  [gbastien]
- Added parameter `replace_not_found_image=True` to `xhtml.storeImagesLocally`,
  when `True` (default) and an image could not be retrieved,
  a `Not found` image will be used. This solves problem when copy/paste a private
  image from another site, available in the browser because of shared
  authentication but not retrievable.
  [gbastien]

#### imio.pyutils (0.22 → 0.23)

#### Version 0.23 (2022-07-01)

- Added `utils.append` to append a value and return it.
  [sgeulette]

#### collective.contact.plonegroup (1.42 → 1.43)

#### Version 1.43 (2022-07-01)

- Added `utils.get_suffixed_groups`.
  [sgeulette]
- Do not delete a group (after a function removal) if not empty
  [sgeulette]

#### collective.contact.widget (1.12 → 1.13)

#### Version 1.13 (2022-06-21)

- Escaped contact title special characters in `term-contact` viewlet to avoid
  script insertion (xss). This viewlet stores an hidden field used in a
  dynamically js generation.
  [sgeulette]
- Require `future` in `setup.py`.
  [gbastien]

#### collective.documentgenerator (3.33 → 3.34)

#### Version 3.34 (2022-06-21)

- Stored `template_uid` on a persistent generated document to know which template has been used.
  [sgeulette]

#### collective.eeafaceted.batchactions (1.10 → 1.11)

#### Version 1.11 (2022-05-06)

- Avoided exception when referer url contains non ascii char.
  [sgeulette]

#### imio.pm.locales (4.2b27 → 4.2b28)

*No changelog entries found.*

#### plonemeeting.restapi (1.0rc15 → 1.0rc17)

*No changelog entries found.*

## Release 4.2.13

**Date:** 2022-06-23

### Package Updates

#### Products.PloneMeeting (4.2rc27 → 4.2rc29)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b20 → 4.2b21)

*No changelog entries found.*

#### appy (1.0.10 → 1.0.12)

*No changelog entries found.*

#### imio.annex (2.17 → 2.18)

#### Version 2.18 (2022-06-14)

- Added `safe_utils.py` that will only include safe utils.
  [gbastien]
- Removed override of columns that was done to use `collective.eeafaceted.z3ctable`
  as now at is already the case.
  [gbastien]

#### imio.helpers (0.56 → 0.58)

#### Version 0.58 (2022-06-14)

- Added `get_zope_root` to get zope app.
  [sgeulette]
- Added `zope_app` parameter in `set_site_from_package_config`.
  [sgeulette]
- Fixed `xhtml.replace_content`, make sure the entire content is replaced
  including sub tags.
  [gbastien]

#### Version 0.57 (2022-06-10)

- Added `NoEscapeLinkColumn` as base for link column rendering html.
  Escape must be done in inherited column.
  [sgeulette]
- `content.uuidToObject` will now return `None` instead an empty list if uuid not found.
  [gbastien]
- Remove zope.app.publication dependency in `security.set_site_from_package_config` as it is now
  removed since Plone >= 5.2.6
  [aduchene]

#### imio.history (1.26 → 1.27)

#### Version 1.27 (2022-06-14)

- Added `safe_utils.py` that will only include safe utils.
  [gbastien]

#### imio.prettylink (1.19 → 1.20)

#### Version 1.20 (2022-06-14)

- Escape link content to avoid malicious behaviour.
  [gbastien]

#### collective.contact.core (1.38 → 1.39)

#### Version 1.39 (2022-06-14)

- Added `safe_utils.py` that will only include safe utils.
  [gbastien]
- Added validation for identifiers token INameTokenTableRowSchema.
  [odelaere]

#### collective.contact.plonegroup (1.40 → 1.42)

#### Version 1.42 (2022-06-14)

- Escape user and group title in `DisplayGroupUsersView`.
  Moreover fixed column to be not sortable.
  [gbastien]
- Added `safe_utils.py` that will only include safe utils.
  [gbastien]
- Corrected error in search: do not pass empty portal_type criteria.
  [sgeulette]
- Added parameter escaped=True in `voc_selected_org_suffix_users` function
  [sgeulette]
- Fixed `@@display-group-users` when organization is not selected in plonegroup
  so there is no linked Plone groups, added tests for it and the
  `@@suborganizations` view (z3ctable displaying organizations contained in
  another organization).
  [gbastien]

#### Version 1.41 (2022-05-06)

- Added adapter with methods to check PloneGroupContact delete and transition.
  [sgeulette]

#### collective.documentgenerator (3.29 → 3.33)

#### Version 3.33 (2022-06-14)

- Added character escaping to avoid xss in `TemplatesTable`
  [sgeulette]
- In `utils.update_oo_config_after_bigbang` don't fail instance start up if
  `update_oo_config` raises an exception.
  [odelaere]

#### Version 3.32 (2022-06-02)

- Added upgrade step to `14` that will add the `oo_port_list` parameter to the registry.
  [gbastien]

#### Version 3.31 (2022-06-01)

- Use appy to load balance on multiple LO server.
  [odelaere]

#### Version 3.30 (2022-05-06)

- Added `iterable_in_columns` (for labels document).
  [sgeulette]
- Added `get_relations` in dexterity
  [sgeulette]
- Use Appy to search and replace in POD templates pod expressions.
  [aduchene]
- .ods POD Templates are now usable with search and replace.
  [aduchene]
- Make sure tmp directory is unique when searching and replacing.
  [aduchene]
- Updated readme
  [Arhell]

#### collective.eeafaceted.z3ctable (2.16 → 2.18)

#### Version 2.18 (2022-06-14)

- Added `BaseColumn.escape = True` so content is escaped.
  Manage escape manually for the `TitleColumn`,  `VocabularyColumn` and the
  `AbbrColumn`, set it to `False` for `CheckBoxColumn`, `ElementNumberColumn`
  and `ActionsColumn` that are entirely generated, set it to `False` for
  `PrettyLinkColumnNothing` as `imio.prettylink` manages it itself.
  [gbastien]

#### Version 2.17 (2022-05-13)

- Doing an unrestricted object get to increase performance.
  [sgeulette]

#### collective.iconifiedcategory (0.53 → 0.54)

#### Version 0.54 (2022-06-14)

- Added `@@categorized-childs-manage` that will render a link to manage
  categorized elements.
  [gbastien]
- Implemented `CategorizedContent._unrestrictedGetObject` as `collective.eeafaceted.z3ctable`
  calls now `item._unrestrictedGetObject` instead `item.getObject` for performance optimization.
  [gbastien]
- Added `safe_utils.py` that will only include safe utils.
  [gbastien]
- We need to escape some content to avoid malicious content:

  - Rely on collective.eeafaceted.z3ctable to display the categorized content table, it manages escaping content;
  - Escape category title in vocabularies.

  [gbastien]

#### imio.pm.locales (4.2b26 → 4.2b27)

*No changelog entries found.*

#### imio.zamqp.pm (0.14 → 0.15)

#### Version 0.15 (2022-06-14)

- In `consumer._manage_after_scan_change_annex_type_to`, set the `content_category`
  on the adapted context (with `IIconifiedCategorization` behavior) so the
  `@content_category.setter` is called and default values are adapted accordingly.
  [gbastien]

#### plone.restapi (7.7.0 → 7.8.0)

*No changelog entries found.*

#### plonemeeting.restapi (1.0rc14 → 1.0rc15)

*No changelog entries found.*

#### plonetheme.imioapps (2.35 → 2.36)

#### Version 2.36 (2022-06-17)

- Do not force an height for img or it hides broken images.
  [gbastien]

## Release 4.2.12

**Date:** 2022-05-17

### Package Updates

#### Products.PloneMeeting (4.2rc20 → 4.2rc27)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b16 → 4.2b20)

*No changelog entries found.*

#### imio.annex (2.15 → 2.17)

#### Version 2.17 (2022-04-26)

- Fixed bug when adding an `annexDecision` because the `content_category`
  could not be retrieved.
  [gbastien]

#### Version 2.16 (2022-04-22)

- Check `validateFileIsPDF` before creating the annex to avoid orphan objects.
  [gbastien]

#### imio.helpers (0.52 → 0.56)

#### Version 0.56 (2022-05-13)

- Added `setup_ram_cache` method.
  [sgeulette]
- Added `set_site_from_package_config` method
  [sgeulette]

#### Version 0.55 (2022-05-06)

- Improved `get_relations` to get optionally referenced objects.
  [sgeulette]

#### Version 0.54 (2022-03-25)

- Added `content.get_vocab_value` based on `content.get_vocab` but returns
  the values (`attr_name='token'` by default, may also be `value` or `title`).
  [gbastien]
- Added `EnhancedTerm` based on `SimpleTerm` providing `attrs` dict on term
  [sgeulette]
- Added `cache.cleanForeverCache` that will clear cache of functions using the
  `@forever.memoize` decorator.
  [gbastien]

#### Version 0.53 (2022-03-17)

- Refactored `get_object`
  [sgeulette]

#### imio.migrator (1.29 → 1.31)

#### Version 1.31 (2022-05-16)

- Added `is_in_part` function to run partially a migration with imio.updates. (See
  FUNC_PARTS in https://github.com/IMIO/imio.updates/blob/master/README.rst)
  [sgeulette]

#### Version 1.30 (2021-11-15)

- Modified `runProfileSteps` method by changing default value of parameter `run_dependencies`.
  Now it's False by default !!
  [sgeulette]
- Added `runProfileSteps` docstring.
  [sgeulette]

#### imio.pyutils (0.18 → 0.22)

#### Version 0.22 (2022-04-28)

- Added `utils.get_clusters` to display a list of number grouped by clusters.
  [gbastien]

#### Version 0.21 (2022-04-26)

- Added `utils.merge_dicts` to be able to merge several dicts for which values
  are list, list are extended in final result.
  [gbastien]

#### Version 0.20 (2022-02-10)

- Modified `memory` to return more useful information.
  [sgeulette]

#### Version 0.19 (2022-01-21)

- Added `process_memory` to return current process memory.
  [sgeulette]
- Added `memory` to return RAM information.
  [sgeulette]

#### collective.contact.plonegroup (1.39 → 1.40)

#### Version 1.40 (2022-04-22)

- Adapted the `PloneGroupUsersGroupsColumn` to display linked group also when
  organization is not selected in plonegroup, this lets display linked Plone groups
  of an organization that was selected then unselected.
  [gbastien]

#### collective.documentgenerator (3.28 → 3.29)

#### Version 3.29 (2022-04-15)

- Method update_oo_config updates all the registry entries for libreoffice server.
  [odelaere]
- Added subscriber to update oo config on process start.
  [odelaere]

#### collective.eeafaceted.batchactions (1.9 → 1.10)

#### Version 1.10 (2022-02-10)

- Corrected UnicodeDecodeError on transition title.
  [sgeulette]

#### collective.eeafaceted.dashboard (0.18 → 0.19)

#### Version 0.19 (2022-05-16)

- Fixed CSS when using `select2 widget`, a small `margin-left` gap was visible
  between the input and the dropdown.
  [gbastien]

#### collective.iconifiedcategory (0.51 → 0.53)

#### Version 0.53 (2022-04-22)

- Make `validateFileIsPDF` invariant check if a `contentType` is directly
  available on data, this avoid checking on the file.
  [gbastien]

#### Version 0.52 (2022-03-22)

- Fixed `metadata.xml` version, set `2103` instead `2101`.
  [gbastien]

#### collective.js.tooltipster (1.6 → 1.7)

#### Version 1.7 (2022-03-22)

- Added new optional parameters for `tooltipster_helper` : `functionPosition_callback`,
  this let's manage tooltipster position manually.
  [gbastien]

#### collective.big.bang (1.0b2 → 1.0.3)

*No changelog entries found.*

#### imio.pm.locales (4.2b23 → 4.2b26)

*No changelog entries found.*

#### plonemeeting.restapi (1.0rc12 → 1.0rc14)

*No changelog entries found.*

#### plonetheme.imioapps (2.30 → 2.35)

#### Version 2.35 (2022-05-17)

- Completed CSS for `livesearch`, make it looks correctly in Chrome too.
  [gbastien]

#### Version 2.34 (2022-05-16)

- Fixed the default Plone `@@search`:

  - Hide the wildcard search madness, do not display a `*`, every searches are
    done wildcard like it is the case in dashboards;
  - Only display link to `Advanced search` in the livesearch response,
    hide the `Show all results`.

  [gbastien]

#### Version 2.33 (2022-04-26)

- Added some margin at right of a tooltipster so it is never sticked to the screen edge.
  [gbastien]
- Make sure very long words are splitted, this is necessary for Firefox where
  a very long word (or a sentence made of words separated by `-` withtout `blank`)
  was not splitted, making a long horizontal scroll appear.
  [gbastien]

#### Version 2.32 (2022-03-22)

- Fix, add margin under a `tooltipster` only if it is not displayed `top`
  or there is space between tooltipster and origin.
  [gbastien]

#### Version 2.31 (2022-03-22)

- Added some margin under a tooltipster so it is never sticked to the screen edge.
  [gbastien]

## Release 4.2.11

**Date:** 2022-03-15

### Package Updates

#### Products.PloneMeeting (4.2b21 → 4.2rc20)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b14 → 4.2b16)

*No changelog entries found.*

#### appy (1.0.9 → 1.0.10)

*No changelog entries found.*

#### imio.actionspanel (1.57 → 1.60)

#### Version 1.60 (2022-02-04)

- Added possibility to force refresh the page after a WF transition even if on a faceted.
  [gbastien]

#### Version 1.59 (2022-01-24)

- In `actions_panel_actions` displaying `object_buttons`, use the link_target
  defined on the action, only set it to `target="_parent"` if nothing defined
  on the action.
  [gbastien]

#### Version 1.58 (2022-01-14)

- Avoid init `member` in `__init__`, that can lead to member being `Anonymous`.
  [gbastien]
- Fixed detection if transition triggered from faceted, use `has_faceted`
  from `imio.helpers`.
  [gbastien]
- Define a with/height in CSS for icons so it can be reused by
  `collective.js.tooltipster` when it computes the size of the tooltipster.
  [gbastien]
- Added CSS id with context `UID` to the `actions_panel` table.
  [gbastien]

#### imio.annex (2.10 → 2.15)

#### Version 2.15 (2022-02-25)

- Register the `ObjectAddedEvent` and `ObjectModifiedEvent` for `IAnnex`
  so it is not called for other interface.
  [gbastien]

#### Version 2.14 (2022-02-03)

- Accurate french translation for `download-annexes-batch-action-but`.
  [gbastien]

#### Version 2.13 (2022-01-24)

- Set `DownloadAnnexesBatchActionForm.MAX_TOTAL_SIZE` to 25Mb.
  [gbastien]
- Explain in Zip download message that browser may ask to accept popup window.
  [gbastien]
- Open file in new window when clicking on file title in annexes table.
  [gbastien]
- Added a `Download` object_buttons displayed in annex actions_panel.
  [gbastien]

#### Version 2.12 (2022-01-21)

- Fixed `utils.get_annexes_to_print`, use image format (`.png`, `.jpg`, ...)
  stored in annex collective.documentviewer annotation to know the path to
  traverse, this is useful in case image format changed in the global settings.
  [gbastien]

#### Version 2.11 (2022-01-03)

- Added `annex.UID` method to speed up getting the UID.
  [gbastien]

#### imio.dashboard (2.8 → 2.9)

#### Version 2.9 (2022-01-07)

- Fixed setup functions changing state of created elements, use
  `imio.helpers.content.get_transitions` instead `portal_workflow.getTransitionsFor`.
  [gbastien]

#### imio.helpers (0.50 → 0.52)

#### Version 0.52 (2022-01-12)

- Added `cache.obj_modified` function that returns max value between
  obj.modified(), obj._p_mtime and __anotations__._p_mtime
  [sgeulette]
- Added `cache.extract_wrapped` function that returns original decorated function.
  Useful to compare cached and non cached results in tests.
  [sgeulette]
- Updated git fetch url
  [sgeulette]

#### Version 0.51 (2022-01-03)

- Added monkey patch to handle SSL mailer on port 465.
  [sgeulette]
- Added `content.base_getattr` method that will `getattr` without acquisition.
  [gbastien]

#### imio.history (1.22 → 1.26)

#### Version 1.26 (2022-03-08)

- Fixed display of actor fullname in `@@historyview`.
  [gbastien]

#### Version 1.25 (2022-03-07)

- Optimized `@@contenthistory` view.
  [gbastien]

#### Version 1.24 (2022-02-25)

- In `content_history` template, only fix date column width,
  for other columns, let the browser optimize it.
  [gbastien]

#### Version 1.23 (2021-04-21)

- Add Transifex.net service integration to manage the translation process.
  [macagua]
- Add Spanish translation
  [macagua]

#### imio.prettylink (1.17 → 1.19)

#### Version 1.19 (2022-01-12)

- Used now `imio.helpers.cache.obj_modified` in `getLink_cachekey` to include
  annotation change in modification date.
  [sgeulette]
- Updated git fetch url
  [sgeulette]

#### Version 1.18 (2021-03-08)

- Improve check for file when adding `@@download` in url.
  [laz, boulch]

#### imio.pyutils (0.15 → 0.18)

#### Version 0.18 (2022-01-12)

- Made `insert_in_ordereddict` python3 compatible.
  [sgeulette]
- Added `odict_pos_key` to get key at position in ordereddict.
  [sgeulette]

#### Version 0.17 (2022-01-04)

- Added `timed` and `ftimed` functions.
  [sgeulette]
- Added OrderedDict for load_var function
  [sgeulette]

#### Version 0.16 (2021-10-27)

- Added `iterable_as_list_of_list` function.
  [sgeulette]
- Added date in runCommand output
  [sgeulette]

#### imio.restapi (1.0a15 → 1.0b1)

*No changelog entries found.*

#### collective.compoundcriterion (0.4 → 0.5)

#### Version 0.5 (2021-04-20)

- Add Transifex.net service integration to manage the translation process.
  [macagua]
- Add Spanish translation
  [macagua]

#### collective.contact.core (1.36 → 1.38)

#### Version 1.38 (2022-02-03)

- Removed useless imports in collective.contact.core.schema.
  Import ContactList or ContactChoice should be done from collective.contact.widget.schema
  [odelaere]
- Added parameter `display_photo_label_on_views` that will display the field photo
  `label` instead of default behavior that is only displaying the photo without label.
  [gbastien]

#### Version 1.37 (2021-10-20)

- Add image path when exporting
  [boulch]

#### collective.contact.plonegroup (1.38 → 1.39)

#### Version 1.39 (2022-02-03)

- Distinguished cached calls in vocabularies.
  [sgeulette]

#### collective.documentgenerator (3.26 → 3.28)

#### Version 3.28 (2022-01-14)

- Added helper `ConfigurablePODTemplate.get_filename` to easily get file filename.
  [gbastien]

#### Version 3.27 (2021-12-06)

- Updated metadata version.
  [sgeulette]

#### collective.eeafaceted.batchactions (1.8 → 1.9)

#### Version 1.9 (2021-12-06)

- Checked permission on context (in ContactBaseBatchActionForm).
  [sgeulette]

#### collective.eeafaceted.collectionwidget (1.11 → 1.14)

#### Version 1.14 (2022-01-10)

- Fixed `utils.getCurrentCollection`, when `collectionUID` retrieved from
  `facetedQuery` form value, we have a list of values.
  [gbastien]

#### Version 1.13 (2022-01-03)

- Use an alias for `__call__` methods that use `ram.cache` in `vocabulary.py`
  this way, the key generated for the `ram.cache` storage is different.
  [gbastien]

#### Version 1.12 (2021-12-06)

- Added `ram.cache` for `CollectionCategoryVocabulary` to avoid query at each
  request as query is using a `sort_on=getObjPositionInParent` which is very slow.
  [gbastien]
- Override `DashboardCollection` query computation that by default in
  `plone.app.contenttypes` and `plone.app.querystring` will arbitrary add a `path`
  index in the query, and again, the `path` index is very slow and just not necessary.
  [gbastien]
- Use unrestricted catalog query when possible.
  [gbastien]
- Optimized the catalog query that compute the `number_of_items` counters.
  [gbastien]

#### collective.eeafaceted.dashboard (0.17 → 0.18)

#### Version 0.18 (2022-01-03)

- Searched unrestrictedly countable tabs.
  [sgeulette]

#### collective.eeafaceted.z3ctable (2.15 → 2.16)

#### Version 2.16 (2022-01-03)

- Added debug mode when displaying results, this will display the time to
  render each cell, each column (total of every cells) and a global table total.
  Just add `debug=true` to the URL
  [gbastien]

#### collective.iconifiedcategory (0.49 → 0.51)

#### Version 0.51 (2022-03-10)

- Updated upgrade step to 2103 (`Add 'last_updated' to categorized_elements`),
  do not stop in case we found a `last_updated` key in `categorized_elements`
  of an element but continue to next element, maybe some elements were updated
  by another part of code.
  [gbastien]

#### Version 0.50 (2022-01-03)

- Use unrestricted catalog query when possible.
  [gbastien]
- For the view that generated the CSS, do the catalog query that gets the categories
  without `path` and `sort_on` as called from portal and order does not matter.
  [gbastien]
- Added `collective.iconifiedcategory.every_categories` and
  `collective.iconifiedcategory.every_category_titles` vocabularies returning
  every possible categories, including not enabled ones. This will be used to
  manage a `MissingTerms` adapter for `z3c.form`.
  [gbastien]
- Fixed view that generates `collective-iconifiedcategory.css`, get every
  categories including ones that are not `enabled`.
  [gbastien]
- Optimized `@@categorized-childs` view, compute everything only one time
  (context url, context UID, ...) and use `python` or `string` in TAL expressions.
  By default call `utils.get_categorized_elements` with `check_can_view=False`.
  [gbastien]
- Added `check_can_view=True` parameter to `utils.get_categorized_elements`.
  This will do the `IIconifiedContent.can_view` check only done when necessary.
  [gbastien]
- Added data `last_updated` to `categorized_elements` to be used for caching.
  Added upgrade step to version `2103`.
  [gbastien]
- Optimized `ram.cache` key for `utils.get_ordered_categories`, cache until
  any category added/deleted/position changed.
  [gbastien]

#### collective.js.tooltipster (1.4 → 1.6)

#### Version 1.6 (2022-02-14)

- Added `passInstanceToCallback` option to be able to pass the tooltipster
  instance to the `functionReady` callback.
  [gbastien]

#### Version 1.5 (2022-01-03)

- Fixed default `zIndex` from `9995` to `11000` so it works correctly
  when displayed in an overlay.
  [gbastien]

#### collective.big.bang (1.0a3 → 1.0b2)

*No changelog entries found.*

#### imio.pm.locales (4.2b15 → 4.2b23)

*No changelog entries found.*

#### imio.pm.ws (3.2 → 3.6)

#### Version 3.6 (2022-03-10)

- Whenever a `ZSI.Fault` error is raised, display also the message in the log manually
  because `z3c.soap` will not display the error string, only the traceback...
  [gbastien]

#### Version 3.5 (2022-01-14)

- Fixed bug in `_createItem` where it could happen that user used `inTheNameOf`
  had cached `_listAllowedRolesAndUsers` resulting in seeing too much or not
  enough in the dashboard.  Accessing an item that should not be displayed ended
  in an Unauthorized though.
  Every method using inTheName of now use
  `setup_user_in_the_name_of`/`teardown_user_in_the_name_of` to handle it correctly.
  [gbastien]

#### Version 3.4 (2022-01-07)

- Fixed call to `tool.isManager` and handle `utils.get_current_user_id`.
  [gbastien]

#### Version 3.3 (2022-01-04)

- Fixed `SOAPView._mayAccessAdvancedFunctionnalities`, call
  `ToolPloneMeeting.isManager` with `ToolPloneMeeting` instance as first arg,
  required now for caching reasons.
  [gbastien]

#### imio.zamqp.pm (0.12 → 0.14)

#### Version 0.14 (2022-01-07)

- Fixed call to `ToolPloneMeeting.isManager`, when called with
  `realManagers=True`, no context can be passed.
  [gbastien]

#### Version 0.13 (2022-01-03)

- Use `notifyModifiedAndReindex(idxs=['scan_id'])` that will only update relevant
  modification data and `scan_id` after barcode inserted in PDF file.
  [gbastien]

#### plone.restapi (7.5.0 → 7.7.0)

*No changelog entries found.*

#### plonemeeting.restapi (1.0rc4 → 1.0rc12)

*No changelog entries found.*

#### plonetheme.imioapps (2.29 → 2.30)

#### Version 2.30 (2022-03-07)

- If current URL contains `preprod`, highlight `portal-header` (turn it red).
  [jjaumotte]
- Reduce size of `h1 title`, in view mode as well as in edit mode (input).
  [gbastien]

#### Products.CPUtils (1.20 → 1.21)

#### Version 1.21 (2022-03-15)

- Modified del_objects.
  [sgeulette]
- Added parameter `removeWsc=1` to `utils.configure_ckeditor`, this will disable
  the WSC link (Spellcheck) in the scayt menu of CKeditor as it is broken for years.
  [gbastien]

## Release 4.2.10

**Date:** 2021-11-26

### Package Updates

#### Products.PloneMeeting (4.2b18 → 4.2b21)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b12 → 4.2b14)

*No changelog entries found.*

#### appy (1.0.8 → 1.0.9)

*No changelog entries found.*

#### imio.actionspanel (1.56 → 1.57)

#### Version 1.57 (2021-11-08)

- Whenever an error occurs in `ActionsPanelView.triggerTransition`, make sure
  we get the error in the returned portal message and log the full traceback
  in the Zope log.
  [gbastien]

#### imio.annex (2.9 → 2.10)

#### Version 2.10 (2021-11-08)

- Display the annex `filename` and `scan_id` in the categorized elemens table
  under the description.
  [gbastien]

#### imio.helpers (0.47 → 0.50)

#### Version 0.50 (2021-11-26)

- Added `content.get_transitions` to be able to get available transition ids
  (as `wfTool.getTransitionsFor` returns a list of dict with transition infos).
  [gbastien]
- Added `adapters.MissingTerms`, a base `z3c.form` missing terms adapter to be
  extended by local packages.
  [gbastien]
- Added cache auto invalidation mecanism when using `cache.get_cachekey_volatile`
  the caller method can be passed, it's name is stored in the volatiles registry
  then when calling `cache.invalidate_cachekey_volatile_for` with
  `invalidate_cache=True`, every cached methods are invalidated from `ram.cache`.
  This will make stale cache be invalidated immediatelly as when a date changed,
  the existing cache is never used again.
  [gbastien]

#### Version 0.49 (2021-11-08)

- Require `plone.api>1.9.1` because we need `content._parse_object_provides_query`.
  This is necessay since we added `content.find`.
  [gbastien]

#### Version 0.48 (2021-10-20)

- Renamed `content.ur_find` to `content.find` with unrestricted parameter.
  [sgeulette]
- Fixed `content.find` to avoid error if corresponding looped object is deleted.
  [sgeulette]

#### imio.restapi (1.0a14 → 1.0a15)

*No changelog entries found.*

#### collective.contact.plonegroup (1.35 → 1.38)

#### Version 1.38 (2021-11-26)

- In `utils.get_organization` and `utils.get_organizations`, query catalog unrestricted.
  [gbastien]
- Removed `uuidToObject` imported from `plone.app.uuid` in `settings.py`,
  we use `uuidToObject` from `imio.helpers`.
  [gbastien]

#### Version 1.37 (2021-10-20)

- Corrected cache invalidation bug, that wasn't done when a previously deactivated
  organisation is reactivated. Invalidate now wider.
  [sgeulette]

#### Version 1.36 (2021-08-27)

- Added logging using `collective.fingerpointing` in the
  `@@manage-own-groups-users` view when a user was added or removed.
  [gbastien]
- Added `available_expr` to the action displaying the `Manage own groups`,
  action will be displayed if at least one value is selected in the
  `groups_management` field in the configuration.
  [gbastien]
- Use `imio.helpers.SortedUsers` vocabulary in the
  `@@manage-own-groups-users` view.
  [gbastien]

#### collective.documentgenerator (3.25 → 3.26)

#### Version 3.26 (2021-11-08)

- Clean notes when creating/editing a `PODTemplate` this way the `search&replace`
  functionnality works as expected:

  - Added `utils.clean_notes`;
  - Clean notes is only done if `odt_file` changed and file is updated only if
    something was cleaned;
  - Moved function `create_temporary_file` from `events.styles_events` to `utils`.

  [gbastien]

#### collective.eeafaceted.dashboard (0.16.1 → 0.17)

#### Version 0.17 (2021-08-27)

- Adapt code to allow override of faceted context
  [mpeeters]
- Fixed bug in JS function `generatePodDocument` that was only taking elements
  of the current dashboard page and no more following pages.
  [gbastien]

#### collective.eeafaceted.z3ctable (2.14 → 2.15)

#### Version 2.15 (2021-11-08)

- Renamed parameter passed to `PrettyLinkWithAdditionalInfosColumn.getPrettyLink`
  from `item` to `obj` as it is actually the `obj` that is received and not the `item`.
  [gbastien]
- Added attribute `PrettyLinkWithAdditionalInfosColumn.ai_included_fields`,
  by default it displayed every non empty fields, with this parameter it is
  possible to select which fields to display.
  [gbastien]

#### collective.js.iframeresizer (0.3 → 0.4)

#### Version 0.4 (2021-11-26)

- Moved to iFrame Resizer 4.3.2.
  [gbastien]

#### imio.pm.locales (4.2b13 → 4.2b15)

*No changelog entries found.*

#### imio.pm.ws (3.0 → 3.2)

#### Version 3.2 (2021-11-26)

- Call `ToolPloneMeeting.get_orgs_for_user` with `the_objects=True/False`
  when relevant as default value changed in `Products.PloneMeeting`.
  [gbastien]

#### Version 3.1 (2021-11-10)

- In `_meetingsAcceptingItems`, log only one time in the Zope log at the end or
  we have the impression that the method was called many times.
  [gbastien]

#### imio.zamqp.core (0.5 → 0.6)

#### Version 0.6 (2021-04-21)

- In `utils.highest_scan_id`, avoid 2 `return` for lisibility.
  [gbastien]

#### imio.zamqp.pm (0.10 → 0.12)

#### Version 0.12 (2021-11-26)

- Use unrestricted catalog query in `AfterScanChangeAnnexTypeToVocabulary`.
  [gbastien]
- Optimize ram.cache for `ToolPloneMeeting.isManager` by calling it with cfg as context.
  [gbastien]

#### Version 0.11 (2021-11-08)

- Fixed `test_store_pod_template_as_annex_temporary_scan_id_batch_action` as
  `MeetingConfig.meetingItemTemplateToStoreAsAnnex` (single value) was renamed to
  `MeetingConfig.meetingItemTemplatesToStoreAsAnnex` (multi valued).
  [gbastien]
- Fixed `test_may_insert_barcode`, now that we use roles
  `Editor/Reader/Contributor` in `MeetingItem` workflow.
  [gbastien]
- Fixed `test_store_pod_template_as_annex_temporary_scan_id_batch_action` broken
  because Meeting moved from AT to DX.
  [gbastien]
- Do not use devpi.imio.be index anymore for buildout.
  [gbastien]
- Factorized use of `DEFAULT_SCAN_ID` in tests.
  [gbastien]

#### plone.restapi (7.3.7 → 7.5.0)

*No changelog entries found.*

#### plonemeeting.restapi (1.0rc2 → 1.0rc4)

*No changelog entries found.*

#### plonetheme.imioapps (2.28 → 2.29)

#### Version 2.29 (2021-11-08)

- Make abbr/acronym tag display better (space between text and dotted border).
  [gbastien]

#### Products.CPUtils (1.19 → 1.20)

#### Version 1.20 (2021-11-08)

- Completed `object_info`, display `UID` and class name
  (as `meta_type` is not more relevant with `DX`).
  [gbastien]

## Release 4.2.9

**Date:** 2021-10-13

### Package Updates

#### Products.PloneMeeting (4.2b14 → 4.2b18)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b11 → 4.2b12)

*No changelog entries found.*

#### imio.helpers (0.45 → 0.47)

#### Version 0.47 (2021-10-13)

- Fixed `content.get_user_fullname` that was breaking when user had no fullname.
  [gbastien]
- Added `content.ur_find` that's the same as api.content.find but unrestrictedly
  [sgeulette]

#### Version 0.46 (2021-09-28)

- Added `xhtml.replace_content` function that will replace the content of given
  XHTML tag with some other content. This relies on package `cssselect` that is
  added as an extra dependency thru `imio.helpers[lxml]`.
  [gbastien]

#### collective.documentgenerator (3.22 → 3.25)

#### Version 3.25 (2021-09-23)

- Use wrapped context of ProxyObject for __unicode__ method.
  Revert __repr__ to default implementation.
  [sdelcourt]

#### Version 3.24 (2021-09-23)

- Require `beautifulsoup4<4.10` in `setup.py` as starting from 4.10.0,
  `beautifulsoup4` is no more compatible with `Python2`.
  [gbastien]
- Pass parameter `html=True` when calling `Renderer` so content is considered
  as html when using `xhtml` function in POD template, some pre-processing is
  applied to ensure that given content is valid xhtml.
  [gbastien]
- Use wrapped context of ProxyObject for __repr__ and __str__ methods.
  [sdelcourt]

#### Version 3.23 (2021-08-09)

- Allow templates selection on the search result before applying the replace.
  [sdelcourt]

#### imio.pm.locales (4.2b10 → 4.2b13)

*No changelog entries found.*

#### plonemeeting.restapi (1.0b2 → 1.0rc2)

*No changelog entries found.*

#### plonetheme.imioapps (2.26 → 2.28)

#### Version 2.28 (2021-10-13)

- Set size of svg content icon in `folder_factories`.
  [gbastien]

#### Version 2.27 (2021-08-27)

- Added some space between input of an AT multiselection widget.
  [gbastien]
- Added borders on fieldset tabs to distinguish them clearlier.
  [sgeulette]
- Removed icons used to manage "More/Less filters" on the faceted search,
  replace it with an "Advanced search" link and a "Search" icon.
  We rely on collective.fontawesome for the "Search" icon.
  [gbastien]
- Removed styles about `enableFormTabbing` displayed on view, this interacts
  when editing an element in an overlay (because parent frame is a view)
  and does not seem used anywhere?
  [gbastien]

#### Products.CPUtils (1.18 → 1.19)

#### Version 1.19 (2021-09-28)

- Added `del_object` to bypass link integrity check.
  [sgeulette]
- Improved `set_attr` to set a None value
  [sgeulette]
- Added `get_user_pwd_hash` and `set_user_pwd_hash` methods
  [sgeulette]
- Added `check_groups_users` method
  [sgeulette]
- Do not break when generating output log in `utils.change_user_properties`,
  in some cases, like when using an LDAP, a `UnicodeDecodeError` may be raised.
  [gbastien]

## Release 4.2.8

**Date:** 2021-09-09

### Package Updates

#### Products.PloneMeeting (4.2b13 → 4.2b14)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b10 → 4.2b11)

*No changelog entries found.*

#### imio.actionspanel (1.55 → 1.56)

#### Version 1.56 (2021-09-09)

- Fixed arrow used in message explaining when a transition is not triggerable.
  [gbastien]
- Prevent double clicks when triggering a WF transition by disabling
  the link for 2 seconds.
  [gbastien]

#### collective.eeafaceted.dashboard (0.16 → 0.16.1)

*No changelog entries found.*

#### imio.pm.locales (4.2b9 → 4.2b10)

*No changelog entries found.*

## Release 4.2.7

**Date:** 2021-07-19

### Package Updates

#### Products.PloneMeeting (4.2b11 → 4.2b13)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b9 → 4.2b10)

*No changelog entries found.*

#### appy (1.0.4 → 1.0.8)

*No changelog entries found.*

#### imio.actionspanel (1.52 → 1.55)

#### Version 1.55 (2021-06-04)

- Implement method `show` when using async like it is already the case when not
  using async to know if viewlet must be shown.
  [gbastien]
- Added `saveHasActions` call in actions_panel_add_content.pt.
  [sgeulette]
- Fixed `actions_panel_arrows.pt` to display the arrows in a table so we avoid
  icons being one under others when there is not enough place to display it,
  actions have to be always on the same line.
  [gbastien]

#### Version 1.54 (2021-04-26)

- Fixed broken JS event on comment popup `Confirm` button to prevent default behavior,
  this probably leads to action not triggered from time to time on `Firefox`.
  [gbastien]

#### Version 1.53 (2021-04-21)

- Fixed `ActionsPanelView.getTransitions` check on transitions to confirm
  informations, do not consider that prefix of given transition to confirm is a
  `meta_type` but consider it as a `class name` as with `dexterity`, the
  `meta_type` is always the same an no more useable to discriminate content.
  [gbastien]
- Added parameter `forceRedirectOnOwnDelete=False` to `ActionsPanelView.__call__`,
  when deleting an element, by default if current context is a faceted,
  the user is not redirected but the page is reloaded, if we are removing the
  page that holds the faceted then we need to redirect.
  [gbastien]
- In JS function `deleteElement`, set `async:true` for the XHR request.
  [gbastien]
- Fixed bug in Firefox not executing the JS `triggerTransition` XHR request when
  `async:true`, this was due to `preventDefaultClickTransition` not applied when
  using the `@@async_actions_panel` in the viewlet displaying actions,
  it was producing a `NS_BINDING_ERROR` because 2 click events were triggered.
  [gbastien]
- When not using the `useIcons` mode (so when using viewlet displaying buttons),
  if no action at all, do not return an empty HTML table, just return nothing.
  This let's hide the entire viewlet when using the `@@async_actions_panel`.
  [gbastien]

#### imio.annex (2.7 → 2.9)

#### Version 2.9 (2021-07-16)

- Override `collective.iconifiedcategory` columns `category-column`,
  `creation-date-column`, `last-modification-column` and `filesize-column` to
  use `collective.eeafaceted.z3ctable` based columns instead the original
  `z3c.table` columns so we have custom CSS classes.
  [gbastien]
- Added `DownloadAnnexesBatchActionForm`, a batch action to download several
  annexes as a Zip file :
  - download is handled by an ajax request;
  - max download size is 50Mb by default.
  [gbastien]

#### Version 2.8 (2021-04-23)

- Fixed `quickupload.ImioAnnexQuickUploadCapableFileFactory` to make sure that
  thread lock is released like it is the case by default in
  `uploadcapable.QuickUploadCapableFileFactory`.
  This should avoid rare cases where instance is stuck while adding an annex.
  [gbastien]

#### imio.helpers (0.38 → 0.45)

#### Version 0.45 (2021-07-16)

- Added `imio.helpers.SortedUsers`, a vocabulary listing users sorted using
  `natsort.humansorted`. We need to rely on `natsort` to handle this.
  [gbastien]
- Fixed bug in JS function `submitFormHelperOnsuccessDefault` called onsuccess
  by `submitFormHelper` to only consider response as a file to return if
  responser header `content-length` is found in request, this avoid returning
  a wrong blob object when called code returns an error message.
  [gbastien]

#### Version 0.44 (2021-06-15)

- In `xhtml.separate_images` be a bit less defensive, too complex cases are
  still ignored but when the `<p>` contains only non textual elements like
  `<br>` or `blanks`, just ignore these elements.
  [gbastien]

#### Version 0.43 (2021-05-31)

- Lowercased email address after validation.
  [sgeulette]
- Fixed `submitFormHelperOnsuccessDefault` JS function to handle binary response
  so it is possible to download the result of the ajax query.
- Added `xhtml.imagesToData` that turns the src of images used in a xhtml
  content from an `http` or equivalent URL to a data base64 value.
  [gbastien]

#### Version 0.42 (2021-04-30)

- Added parameter `filetype='PNG'` to `barcode.generate_barcode` so it is
  possible to use another supported image file format.
  [gbastien]
- Added parameter `replyto` to `emailer.send_email` so it is possible to add
  `reply-to` header in message
  [sgeulette]
- Adapted `content.object_values` and `content.object_ids` to be able to pass
  a single class name or a list of class names like it is the case for
  `objectValues/objectIds`.
  [gbastien]

#### Version 0.41 (2021-04-21)

- Corrected encoding problem in emailer.
  [sgeulette]

#### Version 0.40 (2021-04-01)

- Added `target` option in `object_link` function
  [sgeulette]
- Added a ZPublisher `:json` suffix type converter.
  [gbastien]
- Changed MockMailHost patch to avoid some problems
  [sgeulette]
- Make `xhtml.storeImagesLocally` handle images with `src` using base64 encoded
  data (like `data:image/png;base64,...)`.
  [gbastien]

#### Version 0.39 (2021-02-25)

- Added `validate_email_address` to check email address with a real name part.
  [sgeulette]
- Added `validate_email_addresses` to check email addresses, separated by a comma.
  [sgeulette]
- Added `content.get_modified_attrs`, when called in a `IObjectModifiedEvent`
  handler, will return the list of field names that were actually modified.
  [gbastien]
- Returned email sender error messages.
  [sgeulette]
- Added `content.uuidToCatalogBrain` that is a shortcut to
  `content.uuidsToCatalogBrains` but that will return a single value.
  [gbastien]
- Added `content.object_values` and `content.object_ids` method, equivalent to
  Zope's `objectValues` and `objectIds` but that will check contained element
  class name instead `meta_type` so it works with DX content types where
  `meta_type` is the same for every types.
  [gbastien]
- Added `content.uuidToObject` that is a shortcut to
  `content.uuidsToObjects` but that will return a single value.
  [gbastien]
- Corrected `has_faceted` function call in `submitFormHelperOnsuccessDefault` js
  [sgeulette]
- Reloaded page when `submitFormHelper` is used on a non faceted page
  [sgeulette]
- Added parameter `toggle_type='slide'` to JS helper `toggleDetails`,
  so it is possible to use `slideToggle` (default) or `fadeToggle`.
  `fadeToggle` behaves better when the hidden part contains a sticky element
  (table header).
  [gbastien]

#### imio.history (1.21 → 1.22)

#### Version 1.22 (2021-03-04)

- Changed default to `False` for parameters `checkMayViewEvent=False` and
  `checkMayViewComment=False` of `utils.getLastAction`, this way, we get last
  action even if current user may not, and it is quicker.
  This fix a performance issue in `ImioWfHistoryAdapter.historyLastEventHasComments`
  when called several times.
  [gbastien]
- In `utils.getLastAction`, parameter `action` may be `before_last` and will
  return the before last action if it exists.
  [gbastien]

#### imio.migrator (1.26 → 1.29)

#### Version 1.29 (2021-07-16)

- Log more infos when updating workflows in `Migrator.refreshDatabase(workflows=True)`.
  [gbastien]

#### Version 1.28 (2021-06-04)

- Added parameter `total_number=None` to `utils.end_time`, when an integer
  is given, the generated message will include info about number of elements
  processed per second.
  [gbastien]

#### Version 1.27 (2021-03-24)

- Moved end time computation and display to `utils.end_time` so it is easy to
  reuse in other contexts.
  Display `days/hours/minutes` only if relevant.
  [gbastien]

#### imio.prettylink (1.16 → 1.17)

#### Version 1.17 (2020-10-06)

- Set icons `<img>` tag `width=16px` and `height=16px` to make `tooltipster`
  happy (computed area to display depends on displayed content).
  [gbaastien]

#### imio.pyutils (0.11 → 0.15)

#### Version 0.15 (2021-04-27)

- Added `ln_key` parameter in `read_dictcsv` method.
  [sgeulette]

#### Version 0.14 (2021-04-21)

- Added `read_dictcsv` function.
  [sgeulette]
- Added `utils.replace_in_list` function to ease replacement of values in a list.
  [gbastien]
- Added `safe_encode` function.
  [sgeulette]

#### Version 0.13 (2020-10-07)

- Added `insert_in_ordereddict` function to easier insert a new key at needed position.
  [sgeulette]

#### Version 0.12 (2020-05-19)

- Update syntax for py 3.
  [odelaere]

#### imio.restapi (1.0a12 → 1.0a14)

*No changelog entries found.*

#### collective.behavior.talcondition (0.11 → 0.14)

#### Version 0.14 (2021-06-29)

- Fix pypi broken package
  [boulch]

#### Version 0.13 (2021-06-29)

- Add uninstall profile
  [boulch]
- Add Plone6 compatibily
  [boulch]

#### Version 0.12 (2021-04-20)

- Add Transifex.net service integration to manage the translation process.
  [macagua]
- Add Spanish translation
  [macagua]
- Do not consider the `archetypes.schemaextender` on Plone5.
  [gbastien]
- Adapted code (except, implementer) to be Python3 compatible.
  [gbastien]
- Added parameter `trusted=False` to `utils._evaluateExpression`, this will use
  a trusted expression handler instead the restricted python default.
  [gbastien]

#### collective.contact.core (1.35 → 1.36)

#### Version 1.36 (2021-04-20)

- In vocabulary.OrganizationTypesOrLevels, use `getRequest` instead
  `context.REQUEST` to get the current request, in some case like when using a
  `plone.restapi` endpoint, `context.REQUEST` could not have an `URL`.
  [gbastien]
- Replaced SearchableText indexers by IDynamicTextIndexExtender adapters.
  So another extender using IDynamicTextIndexExtender also works (like
  collective.behavior.internalnumber).
  [sgeulette]

#### collective.contact.plonegroup (1.33 → 1.35)

#### Version 1.35 (2021-05-05)

- Fixed `addOrModifyOrganizationGroups` called when an organization is modified,
  that was creating Plone groups for every suffixes without considering
  `enabled` or `fct_orgs`. Added upgrade step to `v8` that will delete Plone
  groups that were wrongly created.
  [gbastien]

#### Version 1.34 (2021-04-20)

- Fixed `settings.detectContactPlonegroupChange` where sometimes `event.oldValue`
  is None when value is set several times from different testing layers.
  [gbastien]

#### collective.documentgenerator (3.18 → 3.22)

#### Version 3.22 (2021-07-16)

- Added a view to search and replace in POD templates pod expressions `@@collective.documentgenerator-controlpanel`.
  [aduchene]
- Added an helper class `SearchAndReplacePODTemplates` that can search and replace in POD templates pod expressions.
  [aduchene]
- Added tests on search and replace feature.
  [aduchene]
- Added utility classes to search and replace pod expressions in ODT files.
  [sdelcourt]
- Added a script `bin/search_replace` to search and replace in ODT files via CLI.
  [sdelcourt]
- Added some documentation about search and replace feature.
  [aduchene]
- Added `portal` to the default generation context.
  [gbastien]
- Fix style update temporary file directory didn't use CUSTOM_TMP.
  [odelaere]
- Ensure CUSTOM_TMP directory exists before rendering a document.
  [odelaere]

#### Version 3.21 (2021-04-20)

- Added a view to check up every POD templates `@@check-pod-templates`.
  [odelaere]
- Adapted the `@@check-pod-templates` way to `find_pod_templates` to take into
  account current context.  This way, we may check pod templates on a
  particular folder.
  [gbastien]
- Corrected domain
  [sgeulette]
- Don't check by default selection column in dg-templates-listing to avoid
  user error with batch buttons
  [sgeulette]

#### Version 3.20 (2021-03-09)

- Added CSV file support.
  [odelaere]
- Reworked icons to use svg instead of png and have a more consistent set.
  [odelaere]
- Add generated title parameter for PersistentDocumentGenerationView.
  [jjaumotte]

#### Version 3.19 (2020-10-07)

- Prevent "AttributeError" by not render actionpanel's external edit when there is another pod template to use
  [fngaha]
- Use the same default values between controlpanel schema and registry records.
  [odelaere]

#### collective.eeafaceted.batchactions (1.6 → 1.8)

#### Version 1.8 (2021-07-16)

- Highlight message about number of elements that will be updated
  by the action on the popup.
  [gbastien]

#### Version 1.7 (2021-07-16)

- Adapted code to be able to display several tables on same page
  (and so several batchactions viewlets):

  - Added possibility to define the name of the `CheckBoxColumn`
    (still `select_item` by default);
  - Introduce idea of section for the viewlet and the batch actions so it is
    possible to display different actions on different viewlets or different
    views of same context.

  [gbastien]
- Added method `BaseBatchActionForm._final_update` called when every other
  `update` methods have been called.
  [gbastien]
- Added `BaseBatchActionForm.apply_button_title` attribute to formalize
  management of `apply` button title, that will be `Apply` by default but that
  may be changed to fit the current batch action.
  [gbastien]
- Added `DeleteBatchActionForm` a delete elements batch action.
  [gbastien]
- Require `plone.formwidget.masterselect<2.0.0` as it is only for `Plone5.2+/Py3`.
  [gbastien]

#### collective.eeafaceted.dashboard (0.15 → 0.16)

#### Version 0.16 (2021-04-20)

- Avoid double different checks in
  `DashboardDocumentGenerationView._get_generation_context` (one time checked
  on presence of `facetedQuery` in `REQUEST` then if context is
  `IFacetedNavigable`, only check if context is `IFacetedNavigable`).
  [gbastien]
- Adapted `DashboardDocumentGeneratorLinksViewlet` template
  (`generationlinks.pt`) to use svg icons now that it is the case in
  `collective.documentgenerator`.
  Require `collective.documentgenerator>3.19`.
  [gbastien]
- Small fix in faceted criterion CSS to be sure that first value is
  correctly displayed.
  [gbastien]

#### collective.eeafaceted.z3ctable (2.13 → 2.14)

#### Version 2.14 (2021-07-16)

- Fixed the `CheckBoxColumn`, add a name to the select all/nothing checkbox so
  it is possible to have several checkbox columns (on same table or when
  displaying several tables on same page).
  [gbastien]

#### collective.iconifiedcategory (0.48 → 0.49)

#### Version 0.49 (2021-07-16)

- Added possibility to filter displayed categorized elements on any attribute
  of the categorized element.
  [gbastien]
- Rely on imio.helpers because we need the `:json` suffix type converter.
  [gbastien]
- Register the `categorized_content_container_cloned ObjectClonedEvent` handler
  only for `AT IBaseObject` and `DX IDexterityContent` or is is applied also
  for other elements like `portal_type` because it provides `OFS IItem`.
  [gbastien]
- Added specific `collective.iconifiedcategory.belowcategorizedelements` viewlet
  manager just under the categorized elements table that will be displayed if
  table displayed.
  [gbastien]
- Make the `z3c.table CategorizedTable` easy to override by making a
  `BrowserView` out of it.
  [gbastien]
- Adapted `FilesizeColumn` to display total filesize in column header.
  [gbastien]
- Added `soft_warn_filesize`, a CSS class applied to files of more that `1 Mb`
  (like it is already the case for the `warn_filesize` CSS class applied to
  files of more than `5 Mb`).
  [gbastien]
- Removed the `Show details` action, details are always shown, except, for
  display reasons, when more that 2 columns of elements in the popup.
  [gbastien]

#### imio.pm.locales (4.2b8 → 4.2b9)

*No changelog entries found.*

#### imio.pm.ws (2.16 → 3.0)

#### Version 3.0 (2021-07-16)

- Fixed `test_ws_getItemInfosRequest` now that observers may access item since
  WF initial state, make sure we use a member that does not have access to item
  at all and fixed `test_ws_getConfigInfosItemPositiveDecidedStates`, field
  `MeetingConfig.itemPositiveDecidedStates` was removed and is now managed by
  `MeetingConfig.getItemPositiveDecidedStates` method.
  [gbastien]
- Fixed `getItemInfosRequest/getSingleItemInfosRequest` that was breaking when
  no result and `showEmptyValues=0`.
  [gbastien]
- Adapted tests and code regarding fact that Meeting was moved from AT to DX
  (`linkedMeetingUID` index is renamed to `meeting_uid`, `Meeting.date` attribute
  holds a `datetime` instead a `DateTime`, `attendees` related methods use
  snake_case instead camelCase on both `Meeting` and `MeetingItem`,
  every methods on Meeting use snake_case).
  [gbastien]
- Adapted code now that `MeetingItem.getCategory` does only return the real
  category and not the `proposingGroup` when category not used.
  [gbastien]

#### plone.restapi (6.13.8 → 7.3.7)

*No changelog entries found.*

#### plonemeeting.restapi (1.0b1 → 1.0b2)

*No changelog entries found.*

#### plonetheme.imioapps (2.22 → 2.26)

#### Version 2.26 (2021-07-16)

- imioapps : avoid empty blank space at bottom of tooltipster by using
  `height:auto` on tooltispter container.
  [gbastien]

#### Version 2.25 (2021-07-16)

- imioapps : harmonize input border color with `select2` input (a bit darker).
  [gbastien]
- plonemeetingskin : remove defined height for `viewlet-below-content-title`.
  [gbastien]
- imioapps : added delete icon on delete batch action button and
  download icon on download annexes batch action button.
  [gbastien]
- Limit `select_row` column with as much as possible.
  [gbastien]
- imioapps : increased a bit padding bottom between fields on edit forms.
  [gbastien]

#### Version 2.24 (2021-04-21)

- Fixed problems with too high `tooltipster` overflowing the screen,
  fixed a `max-height` so we have a vertical scroll when necessary.
  [gbastien]
- Changed ia.docs footer viewlets
  [sgeulette]

#### Version 2.23 (2021-03-12)

- Display `cursor: pointer;` when hovering a button or a checkbox.
  [gbastien]
- Resized svg documentgenerator icons
  [sgeulette]
- Avoid tooltipster of more than 80% width.
  [gbastien]
- Move urban css and icons to plonetheme.imioapps.
  [sdelcourt]

#### Products.CPUtils (1.17 → 1.18)

#### Version 1.18 (2021-04-21)

- Added Check all catalog intids for registration method
  [fngaha]
- Fix for password validation that was validating the hash
  [bleybaert]
- Added uid method to display current uid
  [sgeulette]
- Modified ged ckeditor configuration
  [sgeulette]
- Added `filtering` option in `configure_ckeditor` method
  [sgeulette]
- Added `target` option in `object_link`
  [sgeulette]
- Added `show_object_relations` method to display zc relations
  [sgeulette]

## Release 4.2.6

**Date:** 2021-02-03

### Package Updates

#### imio.restapi (1.0a11 → 1.0a12)

*No changelog entries found.*

#### plonemeeting.restapi (1.0a6 → 1.0b1)

*No changelog entries found.*

## Release 4.2.5

**Date:** 2021-01-26

### Package Updates

#### Products.PloneMeeting (4.2b7 → 4.2b11)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b7 → 4.2b9)

*No changelog entries found.*

#### imio.actionspanel (1.51 → 1.52)

#### Version 1.52 (2021-01-26)

- Fixed behavior of just reloading the faceted when deleting an element,
  this was broken because behavior between JS and python code changed and the
  user was redirected to the default dashboard.
  [gbastien]

#### imio.helpers (0.36 → 0.38)

#### Version 0.38 (2021-01-06)

- Added `content.normalize_name` that will normalize a given name, this is the
  code used when turning a title to an id when creating a new content.
  [gbastien]

#### Version 0.37 (2020-12-21)

- Added JS function `submitFormHelper` that will submit a given form and
  `onsuccess`, will call the function `onsuccess` in parameter
  (by default, when called in an overlay, will close the overlay and
  reload the faceted navigation).
  [gbastien]
- Added `security.fplog` helper to ease adding a `collective.fingerpointing`
  message to the log.
  [gbastien]
- Added `plone.app.relationfield` as a direct dependency.
  [gbastien]

#### collective.contact.core (1.33 → 1.35)

#### Version 1.35 (2021-01-14)

- Added `utils.get_position_type_name` that will return a `position_type name`
  for a given `directory` and `position_type token`.
  [gbastien]

#### Version 1.34 (2020-10-07)

- Added robot test for collective.contatc.widget 1.12 version.
  [daggelpop]

#### collective.contact.plonegroup (1.32 → 1.33)

#### Version 1.33 (2021-01-06)

- Do not grok the package anymore.
  [gbastien]
- Override vocabulary `PositionTypes` from `collective.contact.core`, when
  `context` out of a directory, get `position_types` from `DEFAULT_DIRECTORY_ID`.
  [gbastien]

#### collective.eeafaceted.batchactions (1.5 → 1.6)

#### Version 1.6 (2020-12-21)

- After action applied, do not reload the entire page,
  just reload the current faceted results.
  [gbastien]
- Use `CheckBoxFieldWidget` instead `SelectFieldWidget` to manage labels to
  (un)select in `LabelsBatchActionForm` to avoid manipulation with
  `CTRL+click` for selection. Adapted and rationalized translations.
  [gbastien]
- Add a `collective.fingerpointing` entry when applying action to know
  which action was applied on how much elements.
  [gbastien]

#### collective.eeafaceted.z3ctable (2.12 → 2.13)

#### Version 2.13 (2021-01-06)

- Added possibility to define a `header_help` message that will be displayed
  when hovering header title.
  [gbastien]
- Added `<label>` tag around input for the `CheckBoxColumn` so it can be syled
  to ease checkbox selection on click.
  [gbastien]

#### collective.iconifiedcategory (0.47 → 0.48)

#### Version 0.48 (2021-01-19)

- Rely on `CategorizedObjectAdapter.can_view` to manage access to a categorized
  element, this way, we may manage usecases where current user does not have
  the `View` permission on the element but access is managed by the `can_view`
  adapter method.
  [gbastien]

#### ftw.labels (1.3.1 → 2.0.1)

#### Version 2.0.1 (2019-11-26)

- Corrected bug when removing multiple personal labels, if one is not assigned.
  [sgeulette]

#### Version 2.0.0 (2019-10-15)

- Replaced string by list parameter in ILabeling pers_update method.
  [sgeulette]

#### imio.pm.locales (4.2b6 → 4.2b8)

*No changelog entries found.*

#### plonemeeting.restapi (1.0a5 → 1.0a6)

*No changelog entries found.*

#### plonetheme.imioapps (2.20 → 2.22)

#### Version 2.22 (2021-01-06)

- imioapps : use `width:auto` for overlay popups and set `max-height: 800px`
  to avoid vertical scroll as much as possible.
  [gbastien]
- imioapps : fix `referencebrowserwidget` batching hover and search button size.
  [gbastien]
- imioapps : make the `hover` on pretty links work again.
  [gbastien]
- imioapps : specifically do not add bottom border on `<tr>` of `<table>` using
  `no-style-table` when class `no-border` is applied on `<tr>` tag.
  [gbastien]
- imioapps : in styles defined to avoid using Firefox default (see version 2.19),
  set a lighter border for input/textarea/...
  [gbastien]
- imioapps : make sure the ajax spinner is displayed hover overlays.
  [gbastien]
- imioapps : make the checkboxes displayed in dashboard `CheckBoxColumn`
  column easier to click.
  [gbastien]
- imioapps : add a specific CSS class on body using JS function when brower is
  using `Chrome/Chromium/Safari` (`using-chrome`) or
  when it is using `Firefox` (`using-firefox`).
  [gbastien]
- imioapps : make the faceted result table header sticky.
  [gbastien]

#### Version 2.21 (2020-10-07)

- imioapps : skin data displayed in `PrettyLinkWithAdditionalInfosColumn` column,
  add some margin between data.
  [gbastien]

## Release 4.2.4

**Date:** 2020-12-08

### Package Updates

#### Products.PloneMeeting (4.2b5 → 4.2b7)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b6 → 4.2b7)

*No changelog entries found.*

#### appy (1.0.3 → 1.0.4)

*No changelog entries found.*

#### imio.actionspanel (1.50 → 1.51)

#### Version 1.51 (2020-12-07)

- Added parameter `view_name="@@delete_givenuid"` to JS functions
  `confirmDeleteObject` and `deleteElement` so it is possible to call another
  view when deleting an element.
  It is also possible to avoid refresh and manage it manually.
  [gbastien]
- Make sure table containing actions does not have any border especially on `<tr>`.
  [gbastien]

#### imio.helpers (0.33 → 0.36)

#### Version 0.36 (2020-12-07)

- Added email functions (`create_html_email`, `add_attachment`, `send_email`)
  to create and send an email with attachments.
  [sgeulette]
- Optimized `xhtml.separate_images`, do only walk the tree if
  it contains images (`img` tag).
  [gbastien]
- Fixed `content.richtextval` `outputMimeType` parameter to use
  `text/x-html-safe` instead `text/html`.
  [gbastien]
- Renamed JS function `loadCollapsibleContent` to `loadContent` as it can be
  used outside of `collapsible` scope.
  [gbastien]

#### Version 0.35 (2020-11-18)

- Added JS helper method `canonical_url` to get the current canonical URL
  so the url of the context when on a view.
  [gbastien]
- In `toggleDetails` JS function, moved the part that does the async load in
  `loadCollapsibleContent` function so it is possible to call if from outside.
  [gbastien]
- Added `get_user_from_criteria` helper method to search users following
  email or fullname
  [sgeulette]
- Added param on `transitions` method, to not warn by default
  [sgeulette]
- Completed `appy_pod` usecases, `font-size 50%/150%`.
  [gbastien]
- Added `catalog.merge_queries` function that merges `plone.app.querystring`
  compatible catalog queries into one single query.
  [gbastien]
- Do not break in `xhtml.storeImagesLocally` if a `NotFound` occurs while
  getting an internal image.
  [gbastien]

#### Version 0.34 (2020-10-16)

- Moved JS function `setoddeven` from `listings.js` to
  `helpers.js` so it is available by default.
  [gbastien]
- Added setup_logger in security module to change logger level (when
  doing `instance run` by example)
  [sgeulette]

#### imio.pm.locales (4.2b4 → 4.2b6)

*No changelog entries found.*

#### plonemeeting.restapi (1.0a4 → 1.0a5)

*No changelog entries found.*

## Release 4.2.3

**Date:** 2020-10-27

### Package Updates

#### Products.PloneMeeting (4.2b3 → 4.2b5)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b4 → 4.2b6)

*No changelog entries found.*

#### imio.history (1.20 → 1.21)

#### Version 1.21 (2020-10-26)

- Added helper `utils.get_all_history_attr` to get every occurence of a given
  `attr_name` in a `history`. This will return every `review_state` from the
  `workflow` history for example.
  [gbastien]

#### collective.contact.plonegroup (1.30 → 1.32)

#### Version 1.32 (2020-10-26)

- Fixed `DisplayGroupUsersView.group_title` when `DisplayGroupUsersView.short=True`
  to only apply if we have a format like `My config (My suffix)` or it removed
  last letter.
  [gbastien]
- Added parameter `PloneGroupUsersGroupsColumn.short=True` so
  `@@display-group-users` is rendered short by default.
  [gbastien]

#### Version 1.31 (2020-10-11)

- Combined v6 and v7 upgrade because it fails coming from v5
  [sgeulette]
- Corrected table class name.
  [sgeulette]

#### collective.contact.widget (1.10 → 1.12)

#### Version 1.12 (2020-10-07)

- Added prefiltering on widgets
  [daggelpop, sgeulette]
- Add Transifex.net service integration to manage the translation process.
  [macagua]
- Add Spanish translation
  [macagua]

#### Version 1.11 (2019-09-20)

- Limit catalog results (with sort_limit) because solr sends None for higher limit results.
  [sgeulette]
- Use contact_source metadata in widget result
  [sgeulette]

#### imio.pm.locales (4.2b3 → 4.2b4)

*No changelog entries found.*

#### plonemeeting.restapi (1.0a3 → 1.0a4)

*No changelog entries found.*

## Release 4.2.2

**Date:** 2020-10-02

### Package Updates

#### Products.PloneMeeting (4.2b2 → 4.2b3)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b3 → 4.2b4)

*No changelog entries found.*

#### imio.helpers (0.32 → 0.33)

#### Version 0.33 (2020-10-01)

- Added `content.get_relations` and `content.get_back_relations` to easily
  get relations and back relations on an object.
  [gbastien]
- Do not break in `xhtml.storeImagesLocally` if image URL
  contains non-ASCII characters.
  [gbastien]
- Added `xhtml.separate_images` that will make sure images are separated in
  different `<p>` to avoid breaking `appy.pod` when using `LibreOffice 6.0.x`.
  [gbastien]

#### imio.history (1.19 → 1.20)

#### Version 1.20 (2020-10-01)

- Added parameters `checkMayViewEvent=False` and `checkMayViewComment=False` to
  `utils.getLastWFAction`, this way, we get last WF action even if current user
  may not, and it is quicker.
  [gbastien]

#### collective.contact.plonegroup (1.29.1 → 1.30)

#### Version 1.30 (2020-10-02)

- Added manage-own-groups-users view and functions/groups selection configuration.
  A user can manage the user assignments of his groups.
  [sgeulette]
- Avoid getting groups (only users) in `get_selected_org_suffix_users` function.
  [sgeulette]
- Avoid GroupNotFoundError in `get_selected_org_suffix_users` if suffix is limited to some organizations.
  [sgeulette]
- Added `BaseOrganizationServicesVocabulary._term_value` and
  `BaseOrganizationServicesVocabulary._term_token` to ease override
  of rendered term value and token.
  [gbastien]
- Make `SelectedOrganizationsElephantVocabulary` inherits from
  `OwnOrganizationServicesVocabulary` so methods `_term_value` and
  `_term_token` are available.
  [gbastien]
- In `@@display-group-users` instead displaying contained groups without
  contained members, display members of contained groups for normal users,
  display contained groups and contained members to Managers.
  [gbastien]
- Fixed `ConnectionStateError` while setting `registry[FUNCTIONS_REGISTRY]`
  in tests and profile is applied several times.
  [gbastien]

#### collective.eeafaceted.dashboard (0.14 → 0.15)

#### Version 0.15 (2020-10-02)

- Fixed pretty link displayed in dashboards, not necessary to change
  `vertical-align` CSS property.
  [gbastien]
- Added total collections results count on folder tabs providing ICountableTab.
  Only manual refresh for now.
  [daggelpop, sgeulette]

#### collective.eeafaceted.z3ctable (2.11 → 2.12)

#### Version 2.12 (2020-10-02)

- In `PrettyLinkWithAdditionalInfosColumn`, use IDataManager to get widget value.
  [gbastien]

#### imio.pm.locales (4.2b2 → 4.2b3)

*No changelog entries found.*

## Release 4.2.1

**Date:** 2020-09-10

### Package Updates

#### Products.PloneMeeting (4.2b1 → 4.2b2)

*No changelog entries found.*

#### Products.MeetingCommunes (4.2b1 → 4.2b3)

*No changelog entries found.*

#### imio.helpers (0.31 → 0.32)

#### Version 0.32 (2020-09-10)

- Log every 1000 elements instead 100 in `catalog.addOrUpdateIndexes` and
  `catalog.reindexIndexes`.
  [gbastien]
- Fixed code to make except Exception syntax Python 3.8 compatible.
  [gbastien]

#### imio.migrator (1.25 → 1.26)

#### Version 1.26 (2020-09-07)

- Log every 1000 elements instead 100 in `Migrator.reindexIndexes` and
  `Migrator.reindexIndexesFor`.
  [gbastien]

#### collective.eeafaceted.dashboard (0.13.2 → 0.14)

#### Version 0.14 (2020-09-10)

- Fixed css of `no results` sentence for `eea.facetednavigation>14`.
  [gbastien]

#### imio.pm.locales (4.2b1 → 4.2b2)

*No changelog entries found.*

#### plonetheme.imioapps (2.18 → 2.20)

#### Version 2.20 (2020-09-07)

- plonemeetingskin : increase base line-height as font-size was increased.
  [gbastien]

#### Version 2.19 (2020-09-01)

- Fix input text/passowrd and textarea background-color so default styles
  applied by Firefox are overrided (Firefox 80+).
  [gbastien]

## Release 4.2.0

**Date:** 2020-08-26

### Package Updates

#### Products.PloneMeeting (4.1.28.35 → 4.2b1)

#### Version 4.2 (2023-03-06)

- Fixed JS that displays/hides other configs to clone to on item edit when
  possible to send to several other configs.
  [gbastien]
- Added parameter `item` to adaptable method
  `MeetingConfig.get_item_custom_suffix_roles`.
  [gbastien]
- Removed `&nbsp;` from committees vocabulary or it is rendered in faceted filter.
  [gbastien]
- Fixed `meetingconfig_view`, moved `usedPollTypes` and `defaultPollType`
  to the `Votes` tab.
  [gbastien]
- Avoid `Unauthorized` when a `MeetingManager` updates a meeting date and this
  trigger an update of items having the date as preferred date and an item is
  not viewable by the `MeetingManager`.
  [gbastien]
- Removed management of `forceRedirectAfterTransition` in `MeetingActionsPanelView`
  as this is now the default behavior implemented in `imio.actionspanel`.
  [gbastien]
- In the advice proposing group comment popup, include advice name for which
  user is adding a comment.
  [gbastien]
- Added `RichText` column `committee_observations` to
  `meeting.committees datagridfield`.
  Added upgrade step to 4205.
  [gbastien]
- Added select/unselect all `attendees/excused/absents/voters` when editing
  meeting attendees (contacts).
  [gbastien]
- Hide the `byebye attendee` action on item attendees management if linked
  secret votes are all encoded.
  [gbastien]
- The `waiting_advices_given_and_signed_advices_required_to_validate` WF adaptation
  depends of the `waiting_advices_given_advices_required_to_validate` WF adaptation.
  [gbastien]
- Fixed `MyItemsTakenOverAdapter.query` that was always using same
  `member_id` because it used `forever_cachekey`, now it is not cached anymore.
  [gbastien]
- Optimized WF adaptation `waiting_advices_given_and_signed_advices_required_to_validate`
  to avoid check if advice is not a finances advice.
  [gbastien]
- Added `renderWidgets` macro that factorize rendering a list of widgets on a DX content.
  [gbastien]
- Fixed the `Update local roles` dashboard batch action to make sure elements
  are computed in the dashboard order.
  [gbastien]
- Fixed copy/paste an image in CKeditor when editing an advice from
  a faceted dashboard. Temporary fixed by overriding `CKeditorView` until it is
  fixed in `collective.ckeditor`.
  [gbastien]
- Fixed meeting `@@actions_panel` caching invalidation when a meeting was removed
  then created again, old cache was still used, base cachekey on meeting UID.
  [gbastien]
- Advice historization is no more using Plone versioning but we use a new
  `imio.history` history called `given_advice`.
  [gbastien]
- Fixed display of `MeetingConfig` contacts related fields that was escaped for
  JS protection purpose but was displaying HTML tags in the UI.
  [gbastien]
- Overrided DataGridField `datagrid_select_cell.pt` to use structure in `view` macro
  so values using HTML are correctly rendered (`MeetingConfig.certifiedSignatures`).
  [gbastien]
- Fixed `MeetingItem.setManuallyLinkedItems` when item created from restapi call
  as item is still not indexed and so not found using a `portal_catalog` query.
  [gbastien]
- Overrided `archetypes.referencebrowserwidget popup.pt` to display elements
  colored following `review_state` and sorted on `modified reversed`.
  [gbastien]
- Set `renderOwnDeleteWithComments=True` for `AdviceActionsPanelView` so when
  deleting an advice, a comment may be entered and it will be historized in the
  item's history.
  [gbastien]
- Make sure item templates managers have access to fields that are restricted to
  `MeetingManagers` when managing the item templates.
  [gbastien]
- Added `committees editors` functionnality:

  - May be enabled in `MeetingConfig.committees enable_editors`;
  - When enabled, will create a Plone group, members of this group will be able
    to edit fields `MeetingItem.committeeObservations` and
    `MeetingItem.committeeTranscript`;
  - New searches `Item of my committees` and `Items of my committees editable`
    are available when committees are used.

  [gbastien]
- Added parameters `field_name=None` to `utils.forceHTMLContentTypeForEmptyRichFields`
  so it is possible to specify field name to initialize when known.
  [gbastien]
- Make `adapters.PMNegativePersonalLabelsAdapter` and
  `adapters.PMNegativePreviousIndexValuesAdapter` inherits from base classes
  `adapters.NegativePreviousIndexValuesAdapter` and
  `adapters.NegativePersonalLabelsAdapter` that were moved to
  `collective.compoundcriterion`.
  [gbastien]
- Added possibility to redefine the `poll_type` on a per vote basis so item and
  votes `poll_type` may be different, this is used to manage case where
  emergency is voted using a public vote on an item using secret `poll_type`.
  [gbastien]
- Make the `review_state_title` column (that translates the review_state title
  instead id) also available for dashboards displaying meetings.
  [gbastien]
- Make sure meeting fieldsets order is correct when a custom field has been
  added to an existing fieldset.
  [gbastien]
- Fixed `meeting.committees` default value, ignore `MeetingConfig.committees`
  that use `enabled="item_only"`.
  [gbastien]
- Finally fixed invalidating meeting `actionspanel` caching when meeting
  contains/does not contain items so the `Delete` action is handled correctly.
  `Meeting.number_of_items` replaced parameter `as_int=False` by `as_str=False`
  as we only want it to be str for JS.
  [gbastien]
- Fixed the `waiting_advices` WFAdaptation that was changing the `from_state title`
  (for example state `proposed`) to the `from_state id` and so losing the custom
  title that could be set in `MeetingConfig.itemWFValidationLevels`.
  [gbastien]
- Added `MeetingItem.votesResult`, a field that will hold a generated text of
  votes result based on `MeetingConfig.votesResultTALExpr` but that is also
  editable when generated text needs to be customized.
  [gbastien]
- Renamed migration helper `Migrator.updateItemColumns` to `Migrator.updateColumns`
  now that it manages meeting related attribute `MeetingConfig.meetingColumns` and
  added parameter `cfg_ids=[]` to be able to apply only for some `MeetingConfigs`.
  Renamed migration helper `Migrator.cleanItemFilters` to
  `Migrator.updateItemFilters` as it manages adding/removing filters.  Added
  parameter `cfg_ids=[]` to be able to apply only for some MeetingConfigs as well.
  [gbastien]
- Added possibility to restrict WF states in which the suffix `_observers`
  have access to items. This rely on `MeetingConfig.itemObserversStates`.
  [gbastien]
- Fixed `Unauthorized` in `toolplonemeeting_view` for `MeetingManagers`
  that are not `MeetingManager` for every `MeetingConfig`.
  [gbastien]
- Highlight marginal notes fieldset legend on item view when it contains text.
  [gbastien]
- Added WFA `hide_decisions_when_under_writing_check_returned_to_proposing_group`
  that will check that there are no more items `Returned to proposing group` when
  publishing decisions.
  [gbastien]
- Make sure a `MeetingCategory` can not be renamed if it is used.
  [gbastien]
- Removed field `MeetingConfig.useGroupsAsCategories`, field `MeetingItem.category`
  is now an optional field managed by `MeetingConfig.usedItemAttributes`.
  [gbastien]
- Fixed `IMeeting.validate_dates` that was failing because `Data` object
  does not behaves the same way when creating or editing a `Meeting`.
  [gbastien]
- Make sure not used fields are not displayed on the meeting view.
  `BaseMeetingView.show_field` ignores not used boolean fields that are `False`
  and special management for `IMeeting.place` field.
  [gbastien]
- Fixed `ItemDocumentGenerationHelperView.print_votes`, make sure voters
  are ordered when `include_voters=True`. Fixed `Meeting._get_contacts` to take
  into account parameter `uids` order when given.
  Fixed `MeetingItem.get_item_votes`, use an `OrderedDict` instead a `Dict`
  to store voters to preserve order.
  [gbastien]

#### Version 4.2rc34 (2022-09-29)

- Fixed meeting creation default `signatories` and `voters` that were displayed
  even when not activated in the configuration because some default values were
  defined on the contacts.
  [gbastien]
- Escape annex and annex_type title in `ContainedAnnexesVocabulary` and
  `ContainedDecisionAnnexesVocabulary` in case it contains malicious code.
  [gbastien]
- Fixed bug where order of annexes of an item sent to another MC was not correct.
  This relies on a change in `collective.iconifiedcategory`,
  adapted `IconifiedCategoryGroupAdapter.get_every_categories`.
  [gbastien]
- Added holidays for 2023.
  [gbastien]
- Added `ToolPloneMeeting.doInvalidateAllCache` that is called by the form in
  the UI and manages the redirect, this avoids having a redirect when
  `ToolPloneMeeting.invalidateAllCache` is called from other parts of the code.
  [gbastien]

#### Version 4.2rc33 (2022-09-22)

- Make `Products.CPUtils` available in tests as it is a dependency installed
  by `metadata.xml`.
  [gbastien]

#### Version 4.2rc32 (2022-09-19)

- Fixed `Products.PloneMeeting.vocabularies.faceted_annexes_vocabulary` to take
  into account every annexes configs, not only the `item_annexes` config.
  [gbastien]
- In Migrate_To_4200 replace `.getMeetingNumber()` in TAL expressions by
  `.meeting_number`.
  [gbastien]
- In `meetingitem_view`, render field proposingGroup by using the vocabulary so
  we have coherence between edit and view and it displays sub organizations correctly.
  [gbastien]
- Moved `MeetingItem.get_attendee_short_title` to `Meeting` and reuse it
  everywhere. Manage `include_voting_group` parameter in the method instead
  having to pass it as parameter.
  [gbastien]
- Fixed bug when an item is sent to another MC automatically, it was actually not
  working because `imio.actionspanel_portal_cachekey` was found in the `REQUEST`,
  so added new key in `disable_check_required_data` in `REQUEST` to disable
  `MeetingItemWorkflowConditions._check_required_data` in this case.
  Also fixed `MeetingItem.cloneToOtherMeetingConfig` that was sometimes
  triggering too much transitions.
  [gbastien]
- Make sure a `held_position` is not deletable when used in
  `MeetingConfig.certifiedSignatures` or in `organization.certified_signatures`.
  Moreover use a simplified vocabulary for these 2 certified signatures fields.
  [gbastien]
- Changed behavior of number of attendees displayed on an item: now it takes
  into account absents on the meeting and not only present on the item.
  [gbastien]
- Make `update-local-roles` batch action available on dashboards displaying meetings.
  [gbastien]
- Added adaptable method `MeetingItem._assign_roles_to_all_groups_managing_item_suffixes`
  to handle cases where there are several groups managing item, by default,
  groups not currently managing item will have `View` access.
- Added item field `marginalNotes` to `MeetingItem._bypass_meeting_closed_check_for`
  so it is still editable by a `MeetingManager` when the meeting is closed.
  [gbastien]
- Display buildout git tag version in Plone control panel.
  [gbastien]
- Added `Products.CPUtils` as a dependency in `metadata.xml` so
  `ExternalMethods` are installed.
  [gbastien]

#### Version 4.2rc31 (2022-08-26)

- Added `Meeting.update_first_item_number` that will manage updating first item
  number of the meeting.  This way the method is callable from a TAL expression
  and we may use it when necessary.
  Moreover, the parameter `get_items_additional_catalog_query={}` will let manage
  cases where items to take into account are not every items but only a subset
  of items.
  [gbastien]
- Added `safe_utils.set_dx_value` that will let set a value for a DX content
  attribute from a `RestrictedPython` call.
  [gbastien]
- Fixed vocabularies using organizations to make sure we can use organizations
  outside my organization, excepted for the `MeetingItem.associatedGroups` field.
  [gbastien]
- Adapted overrided `generationlinks.pt` regarding changes in
  `collective.documentgenerator` (POD templates grouped by title).
  [gbastien]
- Added `_configurePortalRepository` in `setuphandlers.py` to remove default
  Plone types that are versionable (`Document`, `Event`, ...).
  Added upgrade step to 4204.
  [gbastien]
- Added possibility to add images to `MeetingItemTemplate/MeetingItemReccuring`.
  Display the `folder_contents` tab on items of the `MeetingConfig`.
  [gbastien]
- Added possibility to manage order of attendees by item, this is sometimes
  necessary when attendee position changed on an item.
  [gbastien]
- Removed field `MeetingConfig.transitionsForPresentingAnItem` as information is
  in `MeetingConfig.itemWFValidationLevels`, method
  `MeetingConfig.getTransitionsForPresentingAnItem` is kept and does the job.
  [gbastien]
- Display info and warning message when meeting `meeting_number/first_item_number`
  fields are updated, especially when numbering logic is inconsistent because
  the previous meeting numbers are not consistent or when a meeting was deleted.
  Moved boolean field `MeetingConfig.yearlyInitMeetingNumber` to multi select field
  `MeetingConfig.yearlyInitMeetingNumbers` so we may yearly reinit meeting fields
  `meeting_number` and `first_item_number`.
  Fields `Meeting.meeting_number` and `Meeting.first_item_number` are now optional.
  Changed `Meeting.get_previous_meeting` parameter `interval` default value
  from `60` to `180` days.
  [gbastien]
- Make sure dashboard cache is invalidated (etags) when a meeting date changed,
  this is necessary so meeting date faceted filters are correct.
  [gbastien]
- Added adaptable method `MeetingConfig._custom_createOrUpdateGroups` to ease
  a profile adding a custom `MeetingConfig` related group.
  `MeetingConfig._createOrUpdateAllPloneGroups` parameter `only_group_ids=False`
  was renamed to `dry_run_return_group_ids=False`.
  [gbastien]
- Make `ToolPloneMeeting.get_filtered_plone_groups_for_user` org_uids parameter
  optionnal so we may only filter on given suffixes.
  [gbastien]
- Added a user `pmManager2`, `MeetingManager` of `meetingConfig2` for tests.
  [gbastien]
- Added possibility to make a committee selectable only on an item and
  not on a meeting.
  [gbastien]
- Added adaptable method `MeetingItem._annex_decision_addable_states_after_validation`
  that will manage item states in which annex decision may be added after the
  validation process so since the `validated` state until the end of the item WF.
  [gbastien]
- Added WF adaptation `waiting_advices_given_and_signed_advices_required_to_validate`
  that will check if necessary advice reached their WF last step.
  This is an answer to rare case where advice is not given `completely` and item was
  validated, now if advice WF last step was no reached, it will not be possible to
  validate the item.
  [gbastien]
- On the meeting view, when no available items, close the `available-items`
  collapsible so it takes less place and display the number of available items
  like it is already the case for presented items so it is clear why the
  collpasible is closed.
  [gbastien]
- Make `imio.helpers.date.wordizeDate` available in `pm_utils`
  (for POD templates, TAL expressions, ...).
  [gbastien]
- Adapted code to use `imio.helpers.cache.get_plone_groups_for_user` instead
  `ToolPloneMeeting.get_plone_groups_for_user` that is deprecated but kept for
  backward compatibility.
  [gbastien]
- As groups in charge title is escaped to avoid malicious code, render it on the
  item view using `structure` or escaped characters like `'` are displayed with
  their html entity code (`&#x27;`).
  [gbastien]

#### Version 4.2rc30 (2022-07-01)

- Make the `Migrate_To_4200._fixPODTemplatesInstructions`
  `getFirstItemNumber/first_item_number` replacement work for any cases,
  not only for `Meeting` POD templates.
  [gbastien]
- In `Migrate_To_4200._fixPODTemplatesInstructions` manage `display_date`
  instructions.
  [gbastien]
- In `MeetingConfig.getMeetingsAcceptingItems`, moved the `review_states`
  computation logic from `MeetingItem.listMeetingsAcceptingItems` to
  `MeetingConfig._getMeetingsAcceptingItemsQuery` so calling
  `MeetingConfig.getMeetingsAcceptingItems` will always be correct when
  `review_states=[]`.
  This fixes a bug in `imio.pm.ws.soap.soapview.SOAPView._meetingsAcceptingItems`
  that was returning the same meetings accepting items no matter user was
  `MeetingManager` or not (was actually always returning meetings accepting items
  as if user was a `MeetingManager`).
  [gbastien]
- Adaptations to display error message on the field and not at the top of the form:

  - Use a `constraint` instead an `invariant` to validate
    `IMeetingCategory.category_mapping_when_cloning_to_other_mc`;
  - Raise a `WidgetActionExecutionError` instead a `Invalid` for
    `IPMDirectory.validate_position_types`.

  [gbastien]
- Reorganized MeetingItem predecessors/successors related methods, added parameter
  `unrestricted=True` to methods missing it so it can be set to `False` when called
  from `plonemeeting.restapi` to get linked items.
  [gbastien]
- Adapted `MeetingConfig.validate_customAdvisers` so it is possible to remove a
  delay aware adviser config if it was never used and to change the
  `for_item_created_from` if it is not an auto asked advice.
  [gbastien]
- Cleaned `UnrestrictedMethodsView`, splitted it to `ItemUnrestrictedMethodsView`
  and `MeetingUnrestrictedMethodsView` because the `findFirstItemNumberForMeeting`
  method is the only one called with a `Meeting` as context and others need a
  `MeetingItem` as context.
  Renamed `findFirstItemNumberForMeeting` to `findFirstItemNumber`.
  [gbastien]
- Fix to not fail to display advice tooltipster on `itemTemplate` when
  no `proposingGroup` is selected.
  [gbastien]
- Make MeetingManager bypass `MeetingCategory.using_groups` check when cloning
  an item, this way we avoid problems with category not selectable by
  `MeetingManager` leading to items not cloned (recurring items, delayed items, ...).
  Added `MeetingItem.get_successor` helper that will return the last
  (and very often only) successor.
  [gbastien]
- Avoid wrong order in item manually linked items when an item was linked before
  it is presented to a meeting, as items are sorted on meeting date.
  Add items without a meeting date at the top of items so it will be at the top
  when inserted into a meeting.
  [gbastien]
- In `Meeting.validate_dates`, removed check for `start_date > date` and
  `end_date < date`, this could not be the cases sometimes...
  [gbastien]
- Added possibility to encode votes by `voting group` and to encode same votes
  for several items.  Added field `held_position.voting_group`.
  [gbastien]

#### Version 4.2rc29 (2022-06-17)

- In `Migrate_To_4200`, update TAL expressions using
  `updateLocalRoles` to `update_local_roles`.
  [gbastien]
- Import harmless functions from `utils.py` into `safe_utils.py` so it is
  available on `pm_utils` in TAL expressions and POD templates.
  [gbastien]
- Make `organization.get_acronym` return an empty string u'' when acronym is `None`.
  [gbastien]
- In `ToolPloneMeeting.pasteItem`, do not use `proposingGroup` vocab `by_value`
  to get the first user group because `by_value` generates a dict that is not
  ordered, use `_terms` that holds terms ordered.
  [gbastien]

#### Version 4.2rc28 (2022-06-14)

- Back to previous behavior for `MeetingItem.mayTakeOver`, do not check
  `ReviewPortalContent` permission but if some WF transitions are triggerable, indeed
  some transitions may be triggerable even if user does not have the `ReviewPortalContent`
  permission, for example when using the `waiting_advices` WF adaptation.
  [gbastien]
- Added `utils.get_prefixed_gn_position_name` to get a prefixed gendered/numbered
  `position_type` from a list of `contacts` and a `position_type`.
  Factorized code used by `PMHeldPosition.get_prefix_for_gender_and_number`
  into `utils._prefixed_gn_position_name`.
  [gbastien]
- Optimize places where `MeetingConfig.getTransitionsForPresentingAnItem` is used
  (recurrings items, duplicate and validate, send to other MC and present) to
  bypass the entire item validation WF if transition `validate` is available directly.
  [gbastien]
- Added WFAdaptations `transfered/transfered_and_duplicated` that will add a
  `transfer` transition to the `transfered` state to the item workflow.
  This is similar to `accepted_out_of_meeting` but is triggerable by
  `MeetingManagers` if item is sendable to other `MeetingConfigs`.
  [gbastien]
- Added possibility to create user fs directly in content/addUsers.
  [odelaere]
- Avoid having the full `utils.py` files available in POD templates,
  select available functions in a `safe_utils.py` file.
  [gbastien]
- Fixed cachekeys for `ItemToDiscussView` and `ItemIsSignedView`, as path to
  image is cached, we need to check the `portal_url` in the cachekey.
  [gbastien]
- CSS, removed double definition of top margin for `static-infos` section that
  was leading to too much space at the top of item reference in dashboards.
  [gbastien]
- Make `Migrator.updatePODTemplatesCode` output format compatible with `collective.documentgenerator`
  builtin `Search&Replace` or when using `appy.pod` S&R (`collective.documentgenerator>3.30`).
  [gbastien]
- Fixed `utils.transformAllRichTextFields` that was losing the `resolveuid` of
  images for AT types (`MeetingItem`) when parameter `onlyField` was used
  (called from quick edit). Added upgrade step to `4203` to fix this, every items
  since migration to 4200 will be fixed as bug was introduced since version 4200...
  [gbastien]
- Avoid rendering malicious content by escaping places where HTML is rendered.
  [gbastien]
- Fixed an issue in `PMDataChangesHistoryAdapter`. The tooltip was mentioning the wrong actor.
  [aduchene]
- When handling `meeting.first_item_number` on meeting closure, only compute
  number if it is still `-1`, in other cases, do nothing, this will manage the case
  when reinitializing the first item number at the beginning of a new year.
  [gbastien]
- Added `events._invalidateAttendeesRelatedCache` to factorize invalidation of
  attendees related cache. Used by `person/held_position/meeting` to invalidate
  caches when necessary.
  [gbastien]

#### Version 4.2rc27 (2022-05-17)

- Added `Migrate_To_4202._fixPreAcceptedWFA` necessary to fix applications using
  the `pre_accepted WFAdaptation` that was fixed in previous version.
  [gbastien]
- Fixed `@@createitemfromtemplate` that was raising an `Unhautorized` because
  cached result holds the url including the member id and this was failing when
  cache was shared between users having same groups.
  Also fixed constrainTypes on `searches_...` folders of each users to not be able
  to add anything to it.
  [gbastien]

#### Version 4.2rc26 (2022-05-16)

- Moved `IRAMCache` configuration to a cleaner place, the `ZopeProcessStarting` event.
  [gbastien]
- Fixed `portlet quickupload` when used on a `Folder` outside the application
  (like a `Documents` folder managed manually at the root of the site).
  [gbastien]
- Fixed `MeetingItem.showObservations` that is an adaptable method.
  [gbastien]
- Fixed `present` transition sometimes not available in `@@meeting_available_items_view`
  when using the `async_actions` because `MeetingItemWorkflowConditions._publishedObjectIsMeeting`
  was returning `False` even when on a `Meeting`.
  [gbastien]
- Removed `is_in_part` management from `Migrator` as it was moved to `imio.migrator`.
  [gbastien]
- Fixed vocabulary used by the `Taken over by` faceted filter to be able to
  select a value `Nobody` to get items taken over by nobody.
  [gbastien]
- Removed `livesearch` override, now overrided and unified in `plonetheme.imioapps`.
  [gbastien]
- Fixed the `pre_accepted WFAdaptation` that was acting like a decided state
  but actually must behaves like an editable item in a meeting (like `presented`
  or `itemfrozen`) and must be fully editable by `MeetingManagers`.
  [gbastien]

#### Version 4.2rc25 (2022-05-10)

- Completed fix about annex type icon wronlgy displayed in meeting
  `@@categorized-annexes` to users not able to access confidential annexes.
  [gbastien]

#### Version 4.2rc24 (2022-05-10)

- Changed from 90° to 270° image rotation in `BaseDGHV.image_orientation` because it is
  rotated clockwise with imagemagick, in pod templates including annexes.
  [aduchene]
- Manage `MeetingConfig.defaultAdviceHiddenDuringRedaction` when a new advice is added,
  and when advice is asked_again the same way (in the edit form) and display a message
  to the adviser.
  [gbastien]
- Display `global_actions` on the advice view.
  [gbastien]
- Fixed annex type icon wronlgy displayed on meeting view to users not able to
  access confidential annexes. The confidential annexes were not downloadable
  but the annex type icon was display and on hover, the `tooltipster` was empty.
  [gbastien]
- Turned `adaptations.WAITING_ADVICES_FROM_STATES` value
  `use_custom_transition_title_for` from a tuple of transitions ids to a dict
  so it is possible to define an arbitrary new custom title for the transition,
  before it was taking the transition id, now it is possible to override several
  different transition title for same transition id in different workflows.
  [gbastien]
- Completed the `restapi_call` debug mode, log the request `BODY` when request is a `POST`.
  [gbastien]
- Fixed item number input `width` on meeting view, `Chrome` does not hanle `auto` as `FF`.
  [gbastien]
- In `@@load_held_position_back_refs`, the view that show where a hed_position is used,
  do display the `...` only when more than 10 elements found.
  [gbastien]

#### Version 4.2rc23 (2022-05-03)

- Fixed `@@categorized-annexes`, display message
  `The configuration does not let you add annexes.` only if not configured
  both `annex` and `annexDecision` annex types.
  [gbastien]
- Fixed `SelectableAssemblyMembersVocabulary` and `SelectableItemInitiatorsVocabulary`
  vocabulary missing terms management that was not handled correctly and added
  double values that broke the SimpleVocabulary.
  [gbastien]
- Fixed width of item number input on meeting (so when editable) so numbers like
  `238.21` are entirely viewable.
  [gbastien]
- Adapted `utils.get_item_validation_wf_suffixes`, that returns group suffixes
  to give access to when item is at least `validated`, to handle a special usecase:
  when no item WF validation levels are enabled (so item is created in state `validated`)
  the `extra_suffixes` defined on the `itemcreated` level will have read access
  to the item, this let's give read access to suffixes such as `prereviewers` or
  `reviewers` because by default, as not used in the workflow, they would not
  get access to the `validated` item.
  [gbastien]
- Moved `utils.reviewersFor` to `MeetingConfig.reviewersFor`, was done before
  because it was using `config.MEETINGREVIEWERS` constant that could be monkeypatched
  by an external profile, now it auto determinates the values from
  `MeetingConfig.itemWFValidationLevels`.
  Added `MeetingConfig._custom_reviewersFor` to be able to manage
  `MeetingConfig.reviewersFor` manually when `MeetingConfig.itemWFValidationLevels`
  is too complex or when same suffix is used several times at differents steps
  of the item validation WF.
  [gbastien]
- Fixed previous `advice_type` was not displayed when advice is `asked_again`
  and `hidden_during_redaction`.
  [gbastien]

#### Version 4.2rc22 (2022-04-28)

- Adapted `Migrate_To_4200._removeBrokenAnnexes`, check that annex UID is in
  his parent's `categorized_elements`, removes it otherwise.
  [gbastien]
- Reintroduced `PMConditionAwareCollectionVocabulary._cache_invalidation_key`
  override to take user groups into account so cache is invalidated when user groups changed.
  [gbastien]
- Added new field `Meeting.adopts_next_agenda_of`.
  [gbastien]
- Added new field `Meeting.mid_start_date`.
  [gbastien]
- Completed POD templates instructions replacements in `Migrate_To_4200`.
  getExtraordinarySession() -> extraordinary_session
  [aduchene]
- Factorized advice custom informations displayed in the advice popup in the
  `@@advice-infos` view so it can be displayed on the advice object view as well.
  [gbastien]
- Avoid `UnicodeDecodeError` in `MeetingItem._updateAdvices` when comparing old
  and new `adviceIndex`, this may happen with old `adviceIndex` containing the
  `comment` as `str` whereas new value is stored as `unicode`.
  [gbastien]
- Added possibility to execute migrations in several parts.
  Migration to 4200 is adapted to be executed in 3 parts (
  `main`, `update_local_roles`, `update workflow mappings/rebuild catalog`).
  [gbastien]
- Fixed `MeetingItem.validate_proposingGroupWithGroupInCharge` to not let select
  a value for which no group in charge is selected (wrong configuration).
  [gbastien]
- Fixed `utils.sendMailIfRelevant` when `isPermission=True` that was simply broken.
  [gbastien]
- Changed behavior of `MeetingItem.get_representatives_in_charge`, it will return
  `held_position objects`, no more the `MeetingItem.groupsInCharge organizations`.
  [gbastien]
- Set first day of calendar widget on `Meeting` to monday instead sunday (default).
  [gbastien]
- Make sure the advice tooltipster does not overflow the top of the screen,
  this could occur when the browser screen is zoomed.
  [gbastien]
- When `debug=true` is passed as parameter during a `restapi` call, or env var
  `RESTAPI_DEBUG` is set to `True`, the result is fully displayed in the event log.
  [gbastien]
- Added `PloneGroupSettingsOrganizationsValidator` that will check that an
  organization unselected from plonegroup settings is not used as group in charge
  of another organization.
  Renamed `PloneGroupSettingsValidator` to `PloneGroupSettingsFunctionsValidator`.
  [gbastien]
- Fixed the WFAdaptations `return_to_proposing_group_with_last_validation` and
  `return_to_proposing_group_with_all_validations` when there was no user in the
  `_reviewers`, the item could not be sent back to the meeting, now the
  `return_to_proposing_group validation WF` takes the last validation state into account.
  [gbastien]
- In the `@@categorized-annexes`, display a clear message when no annex is
  addable because the `MeetingConfig` is not setup.
  [gbastien]
- Added WFAdaptation `item_validation_shortcuts` that will let users change item
  state to any other item validation state (so between itemcreated and validated)
  depending on their groups.
  Added `MeetingItem._assign_roles_to_group_suffixes` to ease assigning roles
  to suffixes for an organization.
  [gbastien]
- Added `MeetingConfig.getId` with `real_id=False` parameter, this will let get
  the real id when used in some tests where we shuffle the id.
  [gbastien]
- Added new field `MeetingItem.otherMeetingConfigsClonableToFieldDetailedDescription`
  that will fill the `detailedDescription` field when sent to another `MeetingConfig`.
  Adapted templates so adding a new `MeetingItem.otherMeetingConfigsClonableToFieldXXX`
  field is managed automatically.
  [gbastien]
- Moved the MeetingItem `budgetRelated/budgetInfos` fields condition logic to
  `MeetingItem.show_budget_infos` so it is easier to override.
  [gbastien]
- Added `ram.cache` for the `@@createitemfromtemplate` view that is responsible
  for calculating the item templates fancy tree.
  [gbastien]
- In the `@@display-meeting-item-not-present` on the meeting displaying items an
  attendee was not present for, display clusters of items numbers to ease reading
  when an attendee is not present for many items.
  [gbastien]
- Add a no_votes_marker parameter to `BaseDGHV.print_votes`
  [aduchene]

#### Version 4.2rc21 (2022-03-22)

- Fixed display of `overlays` and `tooltipsters` on meeting view in the `iframe`
  displaying available items.
  It was sometimes not completelly displayed, now the iframe will resize correctly.
  [gbastien]
- Make `actionspanel` always visible on `DashboardCollection` and `ConfigurablePODTemplate`.
  [gbastien]
- Update `collective.documentgenerator oo_port` on install and in every migrations.
  [gbastien]
- Handle the `from_migration_to_4200=False` parameter when calling `Migrate_To_4201`.
  [gbastien]

#### Version 4.2rc20 (2022-03-15)

- Added `catalog` to the POD template default generation context.
  [gbastien]
- Completed POD templates instructions replacements in `Migrate_To_4200`,
  manage `displayStrikedAssembly` and new default context value `catalog`.
  [gbastien]
- Fixed `PloneGroupSettingsValidator` that was failing to remove an unused
  suffix because wrong check with _advisers suffix.
  [gbastien]
- Fixed WFAdaptation `returned_to_proposing_group`, proposingGroup member was
  not able to add annexes. Added upgrade step to `4201` to fix item WF
  and update existing items WF role mappings.
  [gbastien]
- Disable the `wsc` plugin in `CKeditor` (add it to `removePlugins`) as the link
  to it does not work anymore in the `scayt` menu of `CKeditor`.
  [gbastien]
- Fixed canceling inline change on an item was failing with continuous spinner
  due to use of GET instead POST method to fetch original data.
  [gbastien]
- Minor CSS fix on person view now that we display the `below-content-title`
  viewlet, the app_parameters fieldset was shifted to the right.
  [gbastien]

#### Version 4.2rc19 (2022-03-10)

- Manage some more POD templates instructions replacements in `Migrate_To_4200`,
  replace `meeting.Title()` by `tool.format_date(meeting.date)` and manage various variants.
  [gbastien]
- Added `meeting` to the POD template default generation context, make also the
  `MeetingConfig` available as `cfg`, was already available as `meetingConfig`.
  [gbastien]
- Fixed possible not persisted `categorized_elements` in `utils.updateAnnexesAccess`,
  as it is an `OrderedDict`, we must set `parent._p_changed = True` manually.
  [gbastien]

#### Version 4.2rc18 (2022-03-08)

- Do not fail in `ToolPloneMeeting.update_all_local_roles` if brain is an orphan,
  just log and continue.
  [gbastien]
- Limit width of tooltipster showing advice inherited from informations.
  [gbastien]
- On item WF transition, reindex the `previous_review_state` index.
  This fixes the `searchcorrecteditems` collection no more working.
  [gbastien]

#### Version 4.2rc17 (2022-03-07)

- Redo release not found on pypi.
  [gbastien]

#### Version 4.2rc16 (2022-03-07)

- Fixed `searchitemstoprevalidate` collection TAL condition,
  state is `prevalidated` not `pre_validated`.
  [gbastien]
- Fixed `PMConditionAwareCollectionVocabulary`, do no more override cachekey
  to cache by groups of user as the url contains the user id or cached value
  would contain another user id.
  [gbastien]

#### Version 4.2rc15 (2022-02-25)

- Make sure item `modified` date is not updated by the `UpdateItemsToReindexView`.
  [gbastien]

#### Version 4.2rc14 (2022-02-25)

- Fixed `MeetingItem.modified` not updated when item cloned.
  [gbastien]

#### Version 4.2rc13 (2022-02-25)

- Changed default position of advice tooltipster on item view so it is
  displayed `bottom` to deal with `readmorable`.
  [gbastien]
- Changed default value for `many_users`, set it to `True` if more than 400 users
  or using `LDAP`, `False` otherwise.
  [gbastien]
- Some styles fixes:

  - Display of static-infos in dashboard the same way as on the item view;
  - Display of table with no border in CKeditor in black;
  - Display advice field name in historized advice popup more clearly.

  [gbastien]
- Fixed `MeetingItem.modified` not updated when item cloned.
  [gbastien]

#### Version 4.2rc12 (2022-02-15)

- Fixed behavior of functional advice workflow (when advice has a real WF with several states):

  - item `indexAdvisers` index was not reindexed when advice review_state state
    changed because `item.adviceIndex` was unchanged.  Added advice `review_state`
    to `MeetingItem.adviceIndex` so it changes when advice `review_state` changes
    and so `MeetingItem._updateAdvices` returns `indexAdvisers` as index to update;
  - notify modified item when advice state changed so caching is invalidated for
    collections counter and item modified date is updated;
  - in `events.onAdviceTransition`, only call `AdviceAfterTransitionEvent` if relevant.

  [gbastien]
- Added `MeetingItem._is_currently_updating_advices` to formalize item period in
  which it is updating advices.
  [gbastien]
- Fixed item to discuss toggle functionnality on item view.
  [gbastien]

#### Version 4.2rc11 (2022-02-14)

- Refactored the `waiting_advices` workflowAdaptation:

  - Moved constants to the dict of `waiting_advices` infos so we have per new
    added state parameters;
  - Manage `crossed` transitions, when several `waiting_advices` states are
    reachable from same origin state, in this case, additional transitions are
    added with a `__to__` suffix;
  - Added parameter `new_state_id` to avoid having a very long id
    (`...__or__...__or__...`).

  [gbastien]
- Optimized advices tooltipster opening, the popup was opened even when hovering
  quickly, now this behaves like the annexes tooltipster.
  [gbastien]

#### Version 4.2rc10 (2022-02-10)

- Fixed `MeetingItem._send_history_aware_mail_if_relevant` when item transition back to
  itemcreated from presented (when using WFAdaptation `presented_item_back_to_itemcreated`).
  More over make it possible for item notifications sent by
  `MeetingItem._send_history_aware_mail_if_relevant` and
  `MeetingItem._send_proposing_group_suffix_if_relevant` to be selected together,
  the second notification will be send only of the first was not sent.
  [gbastien]
- Fixed rare case where `local_roles` for `MeetingConfig` related Plone groups
  (`_meetingmanagers`, `_powerobservers`, ...) were not correctly set on contacts,
  this could happen if Plone group already existed (MeetingConfig created/removed/created).
  [gbastien]
- Moved `_addDecidedState` and `_addIsolatedState` out of
  `adaptations._performWorkflowAdaptations` so it can be imported from outside.
  [gbastien]
- Fixed link to create a new item not displayed even when default item template
  not restricted to groups.
  [gbastien]
- Invalidate item `actions_panel` caching when some user/groups changed.
  [gbastien]

#### Version 4.2rc9 (2022-02-04)

- Fixed bug where a meeting was not correctly reloaded after transition from actions_panel.
  [gbastien]

#### Version 4.2rc8 (2022-02-03)

- For security reason, do no more cache the `image_view_fullscreen` view.
  See https://github.com/plone/Products.CMFPlone/security/advisories/GHSA-8w54-22w9-3g8f.
  [gbastien]
- Some fixes for meeting created using restapi:

  - validation error messages must not be returned as unicode;
  - as the `ObjectCreated` event is called after validation, make sure validation
    does not fail with not found attributes added during ObjectCreated event.

  [gbastien]
- Added new parameter `by_signature_number=False` to
  `Meeting.get_item_signatories`, this will return an ordered dict where key is
  the signature number and values are list of item signatories.
  [gbastien]
- Changed default value for `many_users` and `many_groups`, set it to `False` by
  default except when LDAP is available, in this case, many_users is set to `True`.
  [gbastien]

#### Version 4.2rc7 (2022-01-28)

- Added adaptable method `MeetingItem._bypass_meeting_closed_check_for` that
  will make it possible to control the `MeetingItem.mayQuickEdit`
  `bypassMeetingClosedCheck=False` parameter for a given `fieldName`.
  This solves the `MeetingItem.internalNotes` editable forever that was no more
  editable when meeting was closed.
  [gbastien]
- Enable `display_below_content_title_on_views` and `display_photo_label_on_views`
  in `collective.contact.core` registry parameters.
  [gbastien]

#### Version 4.2rc6 (2022-01-27)

- Display item number before item title on item view when item in a meeting, before,
  the item number was only displayed if item had a reference (meeting at least frozen).
  [gbastien]
- Changed order of reindex in `MeetingItem.cloneToOtherMeetingConfig`, call
  `reindexObject` on new and current item after call to `ItemDuplicatedToOtherMCEvent`
  (was done done before).
  [gbastien]
- Moved fields `internalNotes` and `marginalNotes` at the bottom of item edit/view forms.
  [gbastien]
- Set `plonemeeting.restapi` as a direct dependency in `metadata.xml`
  so it is installed by default.
  [gbastien]

#### Version 4.2rc5 (2022-01-24)

- Fixed `MeetingItem.internalNotes` access when item in a `_waiting_advices` state.
  [gbastien]
- Make the async actions column available on meetings lists.
  Added icons to meetings related actions so it takes less place in actions_panel.
  [gbastien]
- Sort `PMPositionTypesVocabulary` alphabetically.
  [gbastien]

#### Version 4.2rc4 (2022-01-24)

- Completed `Migrate_To_4200._fixPODTemplatesInstructions`.
  [gbastien]
- Added `Download` icon to annex and annexDecision.
  [gbastien]
- Fixed `UpdateItemsToReindexView`, iterating on a `LazyMap` of `brains` into
  which we `reindexObject` lead to incomplete loop (like when deleting
  elements in a loop).
  [gbastien]

#### Version 4.2rc3 (2022-01-21)

- As transitions for presenting an item may vary from an `organization` to another
  (if some suffixes are disabled or some suffixed Plone groups are empty), take it
  into account in `MeetingConfig.getTransitionsForPresentingAnItem` and everywhere
  it is called.
  [gbastien]
- Added possibility to set arbitrary when cloning an item by adding a new parameter
  `item_attrs={}` to `MeetingItem.clone`.
  It is used to set the `preferredMeeting` on the new item when adding recurring
  items to a meeting value is set before the item is reindexed.
  [gbastien]
- Fixed JS error in `deletewholemeeting` action when called from dashboard.
  [gbastien]
- Fixed `MeetingItem.validate_pollType`, do not validate if value did not change,
  this solves `Unauthorized` raised by item editor when item in state
  `returned_to_proposing_group` because AT validates every fields and it is only
  editable by `MeetingManagers` when item is linked to a meeting.
  [gbastien]
- Fixed `migrate_to_4200.MeetingMigrator`, make sure `RichTextValue` is unicode.
  Make sure assembly related methods on meeting and item all return unicode.
  [gbastien]
- Added test for `imio.annex.utils.get_annexes_to_print`, make sure it still work
  even if image format (`png`, `jpg`, ...) changed in global settings.
  [gbastien]

#### Version 4.2rc2 (2022-01-18)

- Fixed `Migrate_To_4200._cleanUnusedPersonsAndHeldPositions`, do not use
  `@@delete_givenuid` that aborts transaction!
  [gbastien]
- Set `Meeting.title` to `required=False` as it is omitted from edit and generated.
  This is useful when creating Meeting from WS call, specifying a title is not required.
  [gbastien]

#### Version 4.2rc1 (2022-01-14)

- Fixed `Migrate_To_4200._cleanUnusedPersonsAndHeldPositions`, can not remove
  elements of the list of brains we are itering on.  Call `@@delete_givenuid`
  with `catch_before_delete_exception=False` so `BeforeDeleteException` is raised.
  [gbastien]
- In `events.onHeldPositionWillBeRemoved` use `held_position.get_full_title`
  instead `held_position.Title` that does not include the person title or the
  `portal_message` is somewhat useless.
  [gbastien]

#### Version 4.2b26 (2022-01-14)

- Added header help for `ItemPrivacyColumn` and `ItemPollTypeColumnNothing`.
  [gbastien]

#### Version 4.2b25 (2022-01-14)

- Set `portlet_todo.title_length` to `100` instead `60` (added
  `_updatePortletTodoTitleLength` migration step in migration to `4200`).
  Also fixed `portlet_todo.render_cachekey` to have a per `MeetingConfig` cache.
  [gbastien]
- Fixed `SelectableCommitteeAttendeesVocabulary.__call__` that was failing when
  `Meeting.committes` enabled and adding a new meeting because context is the parent.
  [gbastien]
- On `held_position` view, display back refs (elements using it) asynchronously.
  Added upgrade step to remove unused `held_positions` that were migrated from
  old `MeetingUsers` during migration from `4.0` to `4.1`.
  [gbastien]
- Display POD template `UID` and `filename` in `MeetingConfig` POD templates page.
  [gbastien]
- Use `catalog.unrestrictedSearchResults` everywhere possible.
  [gbastien]
- Use a RadioFieldWidget for `IAdviceRemoveInheritance.inherited_advice_action`.
  [gbastien]
- Added a column displaying a control to display the `Actions panel`, this way the
  `Actions panel` is only computed when relevant and it takes less place.
  [gbastien]
- Fixed functionnality when going to meeting from item, the faceted orphan
  mechanism was not respected making user redirected to an additional page
  containing only orphans.
  [gbastien]
- Added `Migrate_To_4200._correctAccessToPODTemplates` again...
  [gbastien]
- Turned annex preview format from `png` to `jpg`.
  [gbastien]

#### Version 4.2b24 (2022-01-07)

- Use `pm_technical_index` to store item initiators to speed up removal of
  unused `held_position` or `organization` (before it was necessary to walk
  and wake up every items).
  [gbastien]
- Simplified use of `ToolPloneMeeting.isManager`, a `context` must not be
  passed anymore when using `realManagers=True`, so turned every
  `tool.isManager(tool, realManagers=True)` to `tool.isManager(realManagers=True)`.
  [gbastien]
- Fixed `utils.get_current_user_id` that was simply not working,
  now that it works, we must ensure to protect places where we use `adopt_user`.
  [gbastien]

#### Version 4.2b23 (2022-01-04)

- Fixed order of upgrade steps in `Migrate_To_4200`, make sure item WF is correct
  before executing `_removeBrokenAnnexes` that needs the item `review_state`.
  [gbastien]
- Make sure advice title and actions are correctly displayed in advice popup.
  [gbastien]

#### Version 4.2b22 (2022-01-03)

- Adapted `PMCategoryVocabulary` to take into account new parameter
  `only_enabled=True` introduced in `collective.iconifiedcategory`.
  [gbastien]
- Added parameter `MeetingConfig.enableAdviceProposingGroupComment`, `False` by
  default to be able to enable/disable the advice proposing group comment as it
  is in competition with the workflow confirmation popup and both functionnalities
  should not be enabled togheter.
  [gbastien]
- On the `MeetingConfig` page displaying POD templates, for POD templates reusing
  the `odt_file` of another POD template, display a link the the POD template
  `odt_file` real holder.
  [gbastien]
- Fixed bug where an adviser could add an `annex` or `annexDecision` because
  the role `Contributor` was used for both `Add annexes` and `Add advices`
  permissions.
  A new role `MeetingAdviser` is added to manage the `Add advice` permission.
  [gbastien]
- Added parameter `MeetingConfig.itemLabelsEditableByProposingGroupForever`,
  `False` by default, when set to `True`, the item proposing group editors
  will be able to edit the item labels forever.
  [gbastien]
- Changed default behavior of `MeetingItem.internalNotes`:

  - now internal notes are editable forever by profiles selected in new parameter
    `MeetingConfig.itemInternalNotesEditableBy`.
    A new role `MeetingInternalNotesEditor` is added and manages the view/edit
    permission of field `MeetingItem.internalNotes`;
  - renamed `adaptations.performWorkflowAdaptations` to
    `adpatations._performWorkflowAdaptations` to show that it should not be
    called directly.
  - renamed `MeetingItem.attributeIsUsed` to `MeetingItem.attribute_is_used` so
    the same method is available on `Meeting`, `MeetingItem` and `MeetingAdvice`
    and may be used by `utils._addManagedPermissions`.

  [gbastien]
- Fixed default value of `held_position.position` that was not working when
  using a mount point, use a `@form.default_value` (set to own organization)
  instead passing the default values in the URL when adding a new element
  (`++add++held_position?form.widgets.position=...`).
  [gbastien]
- Added two parameters to `view.print_attendees_by_type` to improve formatting in documents.
  `unbreakable_contact_value` to avoid line break in the middle of a person and `end_type_character`
  to end a attendee type with a specific character.
  [aduchene]
- Added a new boolean field "videoconference" on Meeting schema. When it is set, attendees change
  label to "Connected" and a distinctive icon is shown with imio.prettylink.
  [aduchene]
- Optimized `ram.cache` configuration:

  - Monkeypatched `zope.ramcache.Storage.getEntry` to update timestamp while
    getting an existing entry;
  - Adapted ToolPloneMeeting.get_orgs_for_user to no more return objects as
    it uses `ram.cache`, parameter `the_objects=False` by default now;
  - Adapted `global_cache` settings, set `maxEntries=100000`, `maxAge=2400`,
    `cleanupInterval=600` so cache is kept for a long time.
  - Do not more `ram.cache` `Meeting.query_state` and `MeetingItem.query_state`,
    performance test shows it is not necessary.
  - Use unrestricted catalog query when possible and avoid use of `path` index;
  - Stored meeting number of items in `Meeting._number_of_items` instead
    computing it every times the meeting is displayed;
  - Added ram.cached method `MeetingConfig.getItemAdviceStatesForOrg`, it avoids
    getting the organization, use it everywhere possible.
  - Added `ram.cache` for faceted counters (`PMRenderTermView.number_of_items`);
  - Added `Meeting._may_update_item_references` that holds the logic of updating
    item reference, this avoids to loop on items if reference does not need to be updated.
  - In `MeetingItem.update_local_roles`, only `reindexObjectSecurity` if not
    `triggered_by_transition` as the `WorkflowTool` will also `reindexObjectSecurity`.
  - Adapted item navigation widget to not compute available item number on
    display but only when asking first/previous/next/last item.
  - Make cache more shared on dashboards (prettylink, annexes, advices, actions panel).

  [gbastien]
- Now that the meeting number of items is stored, display it in the dashboards.
  [gbastien]
- Changed default behavior for CKeditor tables management:

  - set `collective.documentgenerator` column modifier to `nothing` by default;
  - added a style `Otpimize column width` to be able to enable LO column width
    optimization on a per table basis.

  [gbastien]

#### Version 4.2b21 (2021-11-26)

- Fixed `utils.sendMailIfRelevant` when using mode `test`.
  [gbastien]
- Fixed `waiting_advices` workflow adaptations, only rely on selected workflow
  adaptations and no more manage the ReviewPortalContent permission.
  Adapted also `MeetingItem.mayAskAdviceAgain` to let the proposingGroup member
  ask advice again when item is in a `_waiting_advices` review state.
  [gbastien]
- Adapted `MeetingConfig.getItemWFValidationLevels` parameter `state` to `states`
  so it is possible to pass several review_states.
  New parameter `return_state_singleton=True`, will do method work like before
  by default.
  [gbastien]
- `Meeting._getGroupManagingItem` parameter `theObject` is now `False` by default.
  [gbastien]
- Moved logic of `Proposing group may change state of waiting_advices item` to
  `MeetingItemWorkflowConditions._userIsPGMemberAbleToSendItemBack` and added
  `MeetingItemWorkflowConditions._userIsPGMemberAbleToSendItemBackExtraCondition`
  so it is easy to override (like it is already the case for the
  `Adviser may send item waiting advices back to proposing group` logic).
  [gbastien]

#### Version 4.2b20 (2021-11-15)

- Rely on `archetypes.schematuning` (thought it was already the case).
  [gbastien]
- Fixed `monkey.validate` (load `monkey` in tests so it is taken into account).
  [gbastien]
- Fixed `UnicodeDecodeError` in `CategoriesOfOtherMCsVocabulary` when a disabled
  category was in a `MeetingConfig` having special characters in it's title.
  [gbastien]
- Do not fail in `PMGenerablePODTemplatesAdapter.get_all_pod_templates` when
  `portal_ploneMeeting` is not available (for example when testing `imio.pm.wsclient`).
  [gbastien]

#### Version 4.2b19 (2021-11-08)

- Adapted display condition of the `searchmyitemstoadvice` dashboard collection
  to make sure it is only displayed if some
  `MeetingConfig.selectableAdviserUsers` are defined.
  [gbastien]
- Adapted `MeetingItem.validate_proposingGroup` to bypass validation for Managers
  as most of time they are member of none group.
  [gbastien]
- Adpated CSS to make sure element in review_state `itemcreated_waiting_advices`
  is displayed in red.
  [gbastien]
- Fixed fonctionnality to go from an item back to the meeting and display the
  item on the correct page, this was not working as expected because faceted
  criteria where not initialized with their default value but with the fallback
  value, for example b_size of 40 was actually set to 20.  Now we just pass the
  `b_start` as an url parameter and we manage it in the `Faceted.Query`
  at faceted initialization time.
  [gbastien]
- Added logging when accessing restapi calls, needed to monkeypatch
  `plone.restapi.services.Service`.
  [gbastien]
- Index annexes `scan_id` in item `SearchableText` like it is already the case
  for annex `title`.
  [gbastien]
- Added possibility for the proposingGroup to add a comment on an advice:

  - comment may be edited only by the proposingGroup as long as item is editable
    or advice is addable/editable;
  - comment is only viewable by advisers of the asked advice (and MeetingManagers);
  - added helper method MeetingItem.is_decided.

  [gbastien]
- Fixed `ToolPloneMeeting.getPloneMeetingFolder` that was not creating a
  `MeetingConfig` folder if an element having same id existed at Plone root or
  in Members (a user having same id as the MeetingConfig).
  [gbastien]
- Added JS function that is triggered when a `MeetingConfig` is saved (edit form)
  to make sure every `InAndOutWidget` values are selected, this avoid losing
  values when user clicked on a value of the right panel of the `InAndOutWidget`.
  [gbastien]
- Fixed `onItemWillBeMoved` event that prevented to delete a `Plone Site`.
  [gbastien]
- Do not add `pm-anonymize` style to CKeditor by default,
  this will only be configured on demand.
  [gbastien]
- Added `the_objects=False` parameter to `ToolPloneMeeting.get_plone_groups_for_user`
  to get `GroupData` instances instead group ids.
  This is used by the `plonemeeting.restapi` `@users` endpoint.
  [gbastien]
- Added `utils.get_annexes_config` function to be able to get the annexes config
  depending on `context` and annex `portal_type`.
  [gbastien]
- Fixed sending a WF transition notification e-mail when actor had
  a special character in it's fullname.
  [gastien]
- Removed reference to `pre_validation` WF adaptation that does not exist anymore,
  adapted code accordingly.
  [gbastien]
- Adapted `ToolPloneMeeting._users_groups_value` returned value and cachekey:

  - before we returned the full users/groups association which may be huge and
    take much RAM, now we only return md5 hash;
  - before the cachekey was for one request now we use the PAS principal
    added/removed from from to invalidate cache.
  - Some performances optimization related to this change:

    - Added caching for vocabularies.PMUsers;
    - Simplified `ToolPloneMeeting.getMeetingConfig`, simple use of aq_acquire is
      the fastest implementation, no need for caching;
    - Do not use `ram.cache` when cache is only living during one request, use an
      annotation on the request or use `ram.cache` to store an intermediate format
      (ids ou paths) as it can not cache real objects;
    - use `utils.get_current_user_id` instead `plone.api.user.get_current` when
      it is possible.

  [gbastien]
- By default when displaying the list of POD templates on the `MeetingConfig`
  (in the `Documents` tab), do not display the POD templates details (every fields)
  as it may be slow, this is only done when needed (click on link `Show details`).
  [gbastien]
- Fixed bug when duplicating an item and using field
  `MeetingItem.proposingGroupWithGroupInCharge`, it could happen that resulting
  item kept the original `proposingGroup` for which current user is not creator
  resulting into an item not viewable or editable.
  [gbastien]

#### Version 4.2b18 (2021-10-13)

- Optimized `MeetingItem.setManuallyLinkedItems` by using cache to get items to
  store and especially data used to sort items by meeting date.
  [gbastien]
- Avoid use of `Member.getProperty`:

  - use `ToolPloneMeeting.getUserName` to get user fullname;
  - monkey patched `MembershipTool.getMemberInfo` to add caching.

  [gbastien]
- Fixed `FolderDocumentGenerationHelperView.get_meeting_assembly_stats`,
  use `imio.helpers.content.uuidToObject` instead `api.content.uuidToObject`
  to be able to use the `unrestricted=True` parameter.
  [gbastien]

#### Version 4.2b17 (2021-09-29)

- Added `MeetingItem.validate_pollType` that relies on
  `ChangeItemPollTypeView.validate_new_poll_type` to make sure that it is not
  possible to break encoded votes from the item edit form.
  [gbastien]
- Fixed `MeetingConfig.listSelectableAdvisers` when an organization does not have
  a `_advisers` Plone group.
  [gbastien]

#### Version 4.2b16 (2021-09-28)

- Renamed `CKeditor` style `Anonymize`, needed to fix
  `Migrator.addCKEditorStyle` to avoid `UnicodeDecodeError` when added
  `CKeditor` style name contains special characters.
  Make also the `CKeditor` styles panel displayed larger.
  [gbastien]

#### Version 4.2b15 (2021-09-28)

- Fixed `PMContentHistoryView.show_history` as it may be called on item or
  meeting, only check if powerobserver is also member of proposingGroup when
  context is an item, nonsense when it is a meeting.
  [gbastien]
- Fixed `MeetingConfig.validate_usedMeetingAttributes` that prevent use of
  fields beginning with `committees_` if field `committees` is not enabled.
  Ignore field `committees_observations` that may be used alone without
  field `committees` being enabled.
  [gbastien]
- Fixed `ItemOptionalAdvicesVocabulary` that was failing when using
  `MeetingConfig.selectableAdviserUsers` and a user fullname contained a
  letter with accent.
  [gbastien]
- Adapted `MeetingConfig.listSelectableAdvisers` to display number of users of the
  `advisers` Plone group so we know if it is relevant to select it,
  especially when using `MeetingConfig.selectableAdviserUsers`.
  [gbastien]
- Parameter `use_safe_html` of `BaseDGHV.printXhtml` is now `False` by default
  as `collective.documentgenerator` call to `appy.pod` `Rendered` sets
  `html=True` that does almost the same (make sure given content is XHTML compliant).
  Added parameter `use_appy_pod_preprocessor=False` to `BaseDGHV.printXhtml`
  so it is possible to enable it when using `printXhtml` in another scope than
  a POD template (in `print_deliberation` for example used to format restapi result).
  [gbastien]
- Completed `MeetingItem.validate_proposingGroup` to check when creating a new item
  if selected proposingGroup if one of the current user.  This is necessary when
  creating an item using plonemeeting.restapi to check that a user is not creating
  an item for a proposingGroup he is not member of.
  [gbastien]
- Moved logic of `BaseDGHV.printXhtml` to `utils.convert2xhtml` so it is easy to
  call from outside code like from `plonemeeting.restapi`.
  [gbastien]
- Completed mail notification sent when an item changed state
  (every `item_state_changed_` like notifications) to add transition title
  (so when an item is proposed, notified users know if it was itemcreated or
  validated before) and to add transition actor and transition comments to
  the mail body.
  [gbastien]
- Fixed `MeetingItem._send_history_aware_mail_if_relevant` that was breaking
  if the `down` transition came from `validated`.
  [gbastien]
- Added holidays for 2022.
  [gbastien]
- Added `Migrator.addCKEditorStyle` helper to ease adding an new CKeditor style.
  [gbastien]
- Added possibility to anonymize a part of a rich text using new added CKeditor
  style `span.pm-anonymize`.
  This is also taken into account when data get using restapi.
  [gbastien]

#### Version 4.2b14 (2021-09-09)

- Fixed an issue in `_migrateItemPredecessorReference` when migrating to 4200.
  [aduchene]
- Added parameter `isUserIds` to `utils.sendMailIfRelevant` so it is possible
  to send an e-mail to arbitrary users.
  Renamed parameter `permissionOrSuffixOrRoleOrGroupIds` to `value`.
  [gbastien]
- Added a field `MeetingConfig.itemPreferredMeetingStates` that allows to set
  selectable preferred meeting states.
  [aduchene]
- Added a helper method `MeetingConfig.listStateIds` to get all state ids
  for a given objectType.
  [aduchene]
- Added possibility to ask advice to specific advisers of a group:

  - Advice is still asked to the entire group but a new search
    `My items to advice` will return items for which current adviser
    advice was asked;
  - A new e-mail notification `You have an advice to give` is added so only
    users to which advice is asked are notified;
  - It is still possible for other advisers to give advice and all advices to
    give are still returned by the `All advices to give` search.

  [gbastien]
- Adapted CSS now that link to enable faceted filters is a simple link,
  no more icons.
  [gbastien]
- Reimplement the meeting deadlines functionnalities, display an icon before
  the item title on meeting view if item was validated after a defined deadline.
  [gbastien]
- Fixed `BaseDGHV.view_print_signatures_by_position` and added a test.
  [aduchene]
- Added parameter `raw=True` to `pm_textarea.get_textarea_value` so it will
  return the raw value by default instead the output that is treated by
  `portal_transforms`, as the `PMTextAreaField` contains plain text, it is useless.
  [gbastien]
- Fixed the default item empty template that was not respecting the
  `MeetingItem.templateUsingGroups` parameter, it is now possible to restrict
  the default item empty template to some groups.
  [gbastien]
- While hidding history link on item to the `powerobservers` (when using field
  `MeetingConfig.hideHistoryTo`), do not hide history if current user is
  `powerobserver` and member of the item proposing group.
  [gbastien]
- Fixed display of `Application parameters` fieldset when adding a new organization
  in an overlay when on `Own organization`, CSS was hidding it wrongly.
  [gbastien]
- When going back to meeting from item, go to the correct faceted page and
  scroll to item position. Same scrolling mechanism is now used when an item is
  decided on a meeting, instead just refreshing the faceted, the faceted is
  refreshed and the screen scrolls to the modified item.
  [gbastien]
- Added 3 new types of events related to items that will trigger a mail being sent:

  - Item state changed, history aware : Notify by mail one specific user (if possible)
    based on the item history.
    For "up" transition, if the item has already been there we notify the user
    that made the next transition at the time.
    If it is the first time the item goes to 'new_review_state',
    we notify the proposing group suffix (except manager) because we can't predict the future.
    For "down" transition, we will notify the user that made the precedent 'leading_transition'
    to 'old_review_state'.
  - Item state changed, notify proposing group suffix : notify by mail the proposing group suffix
    that will take care of this item in the new review state
  - Item state changed, notify proposing group suffix except manager : Same as above except we don't
    notify manager(s)

  [aduchene]
- Completed `MeetingConfig.validate_itemWFValidationLevels` to check that the
  `itemcreated` state always exists as first element (even if may be disabled),
  check also that every `back_transition` back transition identifier starts with
  `back` and that format of identifier columns (`state`, `leading_transition`,
  `back_transition` must be only alphanumeric) is correct.
  [gbastien]
- Simplified `PMAttendeeRedefinePositionTypesVocabulary`, removed override of `_get_person`,
  parent `PMPositionTypesVocabulary` now manages also when `person_uid` found in `REQUEST`.
  This makes the list of positions on the `RedefineSignatoryForm` display the positions
  correctly (not the four valeus separated by pipe).
  [gbastien]
- Added method `ToolPloneMeeting.get_labels` to be able to get `ftw.labels` of
  a given context. It is possible to get every labels, normal labels only or
  personal labels only.
  [gbastien]
- Set `collective.documentgenerator` `column_modifier` parameter to `disabled` by default.
  [gbastien]
- Configure `MailHost` by default to use TLS and queuing.
  [gbastien]
- For field `MeetingCategory.category_mapping_when_cloning_to_other_mc`, display
  also disabled categories in vocabulary so it is visible on category view.
  [gbastien]
- Completed `IEncodeSecretVotes.validate_votes` to ensure values are integers.
  [gbastien]
- Added parameter `MeetingConfig.computeItemReferenceForItemsOutOfMeeting` to
  enable computation of item reference for items decided out of meeting.
  Now item reference is updated when item inserted/removed from a meeting but also
  when back to validated and for transitions deciding out of meeting.
  [gbastien]
- Added helper method `Meeting.is_late` and use it everywhere necessary.
  [gbastien]
- Fixed `MeetingItem._adviceIsViewableForCurrentUser` when a confidential advice
  is not shown to powerobservers, the advisers of the advice have access to the
  advice even if they are also powerobservers.
  [gbastien]
- Removed unused method `MeetingItemWorkflowConditions._check_review_and_required`.
  [gbastien]

#### Version 4.2b13 (2021-07-16)

- Fixed `PMDeleteBatchActionForm._get_deletable_elements`, that was not working
  because `PMDeleteBatchActionForm.get_deletable_elements`
  (with a missing leading `_`) was actually overrided...
  [gbastien]
- Fixed `DisplayAssemblyFromMeetingProvider` used in `ManageItemAssemblyForm`
  to only display default `itemAssembly` if actually used.
  Indeed the form may also be used when using attendees to manage item guests.
  [gbastien]

#### Version 4.2b12 (2021-07-16)

- Adapted code regarding fact that icons used in `collective.documentgenerator`
  are now `.svg` instead `.png`.
  [gbastien]
- Use the `Products.PloneMeeting.vocabularies.everyorganizationsacronymsvocabulary`
  and `Products.PloneMeeting.vocabularies.everyorganizationsvocabulary` for every
  dashboard columns, so no matter selected values are in a configuration that
  changed accross time, values will always be in the vocabularies.
  [gbastien]
- In `MeetingConfig` parameters related to columns displayed in various
  dashboards, display the column name as now several columns may have same name
  (`P.G`. is for `Proposing group` and `Proposing group acronym`).
  [gbastien]
- Define a default value of [] for every `schema.List` fields of contacts
  (`organization`, `person`, `held_position`) and `meetingcategory` so we avoid
  to have a `None` instead an iterable while creating a new element by code.
  [gbastien]
- Fixed `MeetingWorkflowActions.doClose` when
  `MeetingConfig.removeAnnexesPreviewsOnMeetingClosure` is enabled and there is
  no item in the meeting.
  [gbastien]
- Removed parameter `the_objects=False` from `AssociatedGroupsVocabulary` and
  `GroupsInChargeVocabulary`, as these vocabularies are ram.cached, cached
  methods must avoid returning objects.
  [gbastien]
- Optimized cached methods : avoid having objects in cachekeys, this make cache
  size too big, when using `ToolPloneMeeting.isManager`, use `cfg` as `context`
  if available.
  [gbastien]
- Extended `Meeting.get_signature_infos_for` so it is possible to get signature
  infos of every signatories of an item, not only the redefined ones, and added
  parameters `render_position_type=False` and `prefix_position_type=False` so
  it is possible to get the raw `position_type`, or rendered, or rendered and
  prefixed.
  [gbastien]
- Prevent to move the default item template to a subfolder
  (removal was already managed, now moval is not possible neither).
  [gbastien]
- Display a help message on the item view regarding copy groups to know in
  which states copy groups will have access to the item.
  [gbastien]
- Migrate `Meeting` from AT to DX :

  - Rely on `collective.dexteritytextindexer` to manage `SearchableText`;
  - Do not use `meta_type` anymore as it is always the same when using
    `dexterity`, rely on `getTagName` from `OFS` that returns the
    `__class__.__name__`;
  - Renamed `Meeting.queryState` and `MeetingItem.queryState` to `query_state`;
  - Moved every `Meeting` related methods from `camelCase` to `snake_case`,
    including most of methods in `MeetingItem` having a direct link with
    `Meeting` (`get_item_attendees`, `get_item_absents`, ...) but not methods
    that are accessors (`MeetingItem.getItemAssembly`,
    `MeetingItem.getItemAssemblyAbsents`, ...);
  - Removed `MeetingItem.displayStrikedItemAssembly`, use
    `MeetingItem.get_item_assembly(striked=True)`;
  - Removed unused methods on MeetingItem (getSpecificMailContext,
    includeMailRecipient, getAssembly, lastValidatedBefore);
  - Do no more display the `assembly` fields on `MeetingItem` edit form
    (`assembly`, `assemblyAbsents`, ...) this allows removal of description
    methods (`ItemAssemblyDescrMethod`, `ItemAssemblyExcusedDescrMethod`, ...);
  - Removed `MeetingConfig.deadlineFreeze` and `MeetingConfig.deadlinePublish`
    related functionnality;
  - Manage `MeetingItem.preferredMeeting` link manually by storing the path to
    the meeting so it allows to reindex the `preferred_meeting_date` when full
    reindexing the portal_catalog (in this case, the preferred meeting could
    not be already indexed and findable in the catalog);
  - Moved `ToolPloneMeeting.formatMeetingDate` to `ToolPloneMeeting.format_date`;
  - Renamed some indexes : `linkedMeetingDate/meeting_date` and
    `getDate/meeting_date` we have now one single index used by the `Meeting` or
    the `MeetingItem`, `getPreferredMeetingDate/preferred_meeting_date`,
    `getPreferredMeeting/preferred_meeting_uid`;
  - Display global action on the meeting_view (collapse all/top/bottom);
  - Removed `@@meeting-before-faceted-infos` and `@@meeting-after-faceted-infos`
    that are no more necessary now that the meeting view template should never
    by overrided anymore, everything is done using the schema and fieldsets
    definition;
  - Most of `Meeting` data is displayable in dashboards displaying meetings as
    static column in the Title column;
  - Added field `Meeting.meetingmanagers_notes` like it exists for `MeetingItem`.

    [gbastien]
- Highlight (bold) the default item template in the itemtemplates folder.
  [gbastien]
- Use `imio.history.utils.getLastWFAction` parameter `transition='before_last'`
  to get the before last `review_state` in `indexes.previous_review_state`.
  [gbastien]
- Fixed `ItemsToAdviceWithoutHiddenDuringRedactionAdapter` that was using the
  same cached method as parent `ItemsToAdviceAdapter` because an alias for query
  was not defined. In this case, the 2 queries return the same result...
  Added a test that checks that a different alias is used for every
  `CompoundCriterionBaseAdapter` query.
  [gbastien]
- Fixed bug in `@@advices-icons` view, a delay icon was wronlgy displayed for
  a non delay-aware advice if a delay-aware advice of same type (positive,
  asked_again, ...) and `hidden_during_redaction` exists on the item.
  Use `MeetingItem.getAdviceDataFor` instead accessing the
  `MeetingItem.adviceIndex` directly as it manages `hidden_during_redaction`
  advice type correctly.
  [gbastien]
- Completed the `DX quick edit RichText field` to manage :

  - `locking` (not being able to edit if another user is editing), hide the edit
    icon if context is locked, if user edit and content is locked in between,
    the page is reloaded;
  - `formUnload` (not losing changes during edition and clicking leaving current page);
  - when quick editing a RichText field, hide the `actions_panel` viewlet, on views
    where it is sticky, it may be confusing and taken for save/cancel controls.

  [gbastien]
- Added `Meeting.committees` management:

  - Committees are defined in `MeetingConfig.committees` datagridfield;
  - When an new meeting is created, `Meeting.committees` is filled using the
    `MeetingConfig.committees` defined values, it manages `date`, `convocation_date`,
    `place`, `assembly/signatures` or `attendees/signatories`;
  - A `MeetingItem.committees` field is added and vocabulary is generated
    from values defined in `MeetingConfig.committees`;
  - It is possible to select committees for an item manually using a multiselect
    or automatically based on the `proposingGroup/category/classifier` of the item;
  - Printing helpers (`printAssembly`, `print_attendees`,
    `print_signatures_by_position`, and `print_signatories_by_position`) have a
    new `committee_id` parameter.

  [gbastien]
- Use the classic `floppy disk save icon` to save item number value when
  changing it on the meeting view instead the `reorder icon` (arrow up and down)
  that was sometimes not clear enough for some users.
  Moreover, added a `Cancel` icon that will hide the icons and set back original
  value to the `itemNumber input`.
  [gbastien]
- Improved `print_signatories_by_position` to be able to use a scanned signature
  and an abbreviated person firstname.
  [aduchene]
- Factorize annexes boolean indexes (`to_print`, `publishable`, `confidential`,
  ...) in `annexes_indexes`, removed `hasAnnexesToPrint/hasAnnexesToSign` index
  and related faceted filter, added a single `Annexes` faceted filter.
  [gbastien]
- Use `SortedSelectedOrganizationsElephantVocabulary` vocabulary instead
  `organization_services` vocabulary from `collective.contact.plonegroup` for
  `category.groups_in_charge` and `organization.groups_in_charge` so elements
  are sorted alphabetically to ease management.
  Vocabulary `organization_services` is no more used in PloneMeeting.
  [gbastien]
- Removed the `@@check-pod-templates` view, we use the one from
  `collective.documentgenerator` that does the same.
  [gbastien]
- Removed `MeetingItem.predecessor` `ReferenceField`, manage
  `predecessor/successors` manually, this will help migrating to DX.
  [gbastien]
- Fixed bug in `ToolPloneMeeting.validate_holidays` that was not catching a
  wrong date format like `20/01/20`.
  [gbastien]
- Hide the `Add MeetingConfig` link on the `portal_plonemeeting` view to non
  Zope admins, this avoid a `siteadmin` adding a `MeetingConfig`.
  [gbastien]
- Integrated `CKeditor imagerotate` plugin to let rotate image when necessary.
  [gbastien]
- Display `imio.pm.ws/plonemeeting.restapi` versions in `@@overview-controlpanel`.
  [gbastien]
- Renamed `ItemDocumentGenerationHelperView.output_for_restapi` to
  `ItemDocumentGenerationHelperView.deliberation_for_restapi`.
  Also added parameter `deliberation_types` to the method to only get relevant
  deliberation variants.
  [gbastien]
- Fixed CSS, avoid horizontal overflow with very large values,
  use `word-break: break-word;`.
  [gbastien]
- Fixed `AskedAdvicesVocabulary` that was sometimes returning terms as being
  inactive because disabled in `MeetingConfig.customAdvisers` but that were
  actually still active because used in `MeetingConfig.selectableAdvisers`.
  [gbastien]
- Fixed `DataGridField` data lost for fields using single checkbox and multi
  checkboxes when validation failed.  This was impacting the `MeetingConfig`.
  Needed to override relevant datagrid templates.
  [gbastien]
- Changed behavior of `MeetingConfig.transitionsReinitializingDelays`:

  - Only reinitialize delay if advice was not given;
  - Optional functionnality `asked_again` is now no more optional;
  - If a given advice must be reinitialized, it must be `asked_again`.

  [gbastien]
- Added possibility to redefine an attendee position on an item.
  Added parameter `MeetingConfig.selectableRedefinedPositionTypes` to be able to
  restrict selectable position_types, if nothing selected, every `position_types`
  defined on the `Contacts` directory are selectable.
  [gbastien]
- On advice popup, when hovering the `user icon`, display every group suffixes
  related to the advice workflow, indeed there may be more than just the
  `_advisers` suffixed group.
  [gbastien]
- Use multiselect widget faceted filters when necessary, handy for replacement
  of checkbox widgets having too much values.  Also make the faceted meeting
  dates display dates with short format (number of month instead name of month).
  [gbastien]
- Added `BaseDGHV.print_scan_id_barcode` to print a barcode in a POD template,
  moreover it will take care that a barcode is not generated more than one time
  for a given context, this avoid cases where barcode is generated several
  times by mistake, that makes the reimport process fail.
  [gbastien]
- Display a warning on the meeting view next to `Assembly and signatures` when
  a signatory is missing, this often leads to broken POD templates.
  [gbastien]
- Do not break in `MeetingItem.getGroupsInCharge` when `includeAuto=True`,
  `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup=True` and no
  `proposingGroup` is defined on the item, this may be the case on an item template.
  [gbastien]
- Fixed `SelectableCommitteesVocabulary` that was failing when adding several new
  `MeetingConfig.committees` (in this case, terms with token '' were generated
  and it failed with `ValueError: term values must be unique: ''`).
  [gbastien]
- Fixed `Meeting.place` MasterSelect widget when `MeetingConfig.places` contains
  special characters.
  [gbastien]
- Change default period for faceted date widgets from
  `-10 years/+10 years` to `-30 years/+2 years`.
  [gbastien]
- Minor fixes in votes :

  - Display number of not encoded votes when using several linked secret votes
    or it was necessary for now to compute it mentally...;
  - Fixed bug in `@@display-meeting-item-voters` considering secret linked
    votes as not complete when using more than 2 linked votes;
  - Display `MeetingItem.pollType` field if enabled or when votes are enabled;
  - Added validation for `MeetingConfig.defaultPollType`
    (must be among MeetingConfig.usedPollTypes);
  - Added validation for `MeetingConfig.firstLinkedVoteUsedVoteValues` and
    `MeetingConfig.nextLinkedVotesUsedVoteValues`
    (must be among `MeetingConfig.usedVoteValues`).

  [gbastien]
- Fix access to annexes of inherited advice when original advice is not viewable
  by current user (for example when item sent from MeetingConfig A to B and user
  is power observer of MeetingConfig B, he does not have access to original
  item/advice/annex stored in MeetingConfig A).
  As advice full preview is not available neither, implemented a
  `Read more/Read less` functionnality to be able to see full `comment/observations`
  in advice popup.
  [gbastien]
- Use search&replace from collective.documentgenerator in migration to 4200:

  - Added migration helper `Migrator.updatePODTemplatesCode`;
  - Added helper `MeetingItem.get_representatives_in_charge` that returns
    representatives in charge of an item;
  - Added `BaseDGHV.print_value` to be able to render any stored field in
    POD templates (`datetime`, `RichText`, `List/Choice` with `vocabulary`, ...);
  - Fixed `actions_panel` on element of the configuration.

  [gbastien]
- Let add a new `held_position` directly from the dashboard displaying persons
  (display the `Add content` action in icons actions panel for `person`).
  [gbastien]
- Added `marginalNotes_column` to `MeetingConfig.listItemRelatedColumns` to be
  able to display the `MeetingItem.marginalNotes` field as static info
  (always visible in Title column) in the dashboards.
  [gbastien]
- Fixed `MeetingItem._check_required_data` to check that `MeetingItem.groupsInCharge`
  is set when using `MeetingItem.proposingGroupWithGroupInCharge`.
  It may happen that `MeetingItem.proposingGroup` is set but not
  `MeetingItem.groupsInCharge` when item is created using a WS call.
  [gbastien]
- Adapted behavior of `MeetingItem._check_required_data`, when the transition is
  computed for the actions_panel, every destination states are checked, if
  transitions are triggered by code (WS call, item sent to another MC, ...)
  then only the `presented` destination state is checked.
  [gbastien]
- Fixed `AskedAdvicesVocabulary` that was not displaying advisers that were only
  defined as power advisers.
  [gbastien]
- Removed the `MeetingItem category/proposingGroup` magic that was relying on
  `MeetingConfig.useGroupsAsCategories`.
  `MeetingItem.getCategory` does not care anymore about proposingGroup and will
  return an empty string or the stored category id.
  [gbastien]
- Fixed `ToolPloneMeeting.pasteItem` that was not correctly removing `sent item
  to another MC` related annotations when item was sent to several other MCs.
  [gbastien]
- Added parameter `image_src_to_data=False` to `BaseDGHV.printXhtml` to be able
  to turn images src to base64 data value using `imio.helpers.xhtml.imagesToData`.
  Also added values `deliberation_motivation` and `deliberation_decision` to
  possible values returned by `ItemDocumentGenerationHelperView.deliberation_for_restapi`.
  [gbastien]
- Enabled batch actions on annexes:

  - Batch actions `Delete` and `Download as Zip` are available;
  - Added `MeetingConfig.enabledAnnexesBatchActions` attribute to be able enable
    or disable batch actions, by default only the `Download` action is enabled.

  [gbastien]
- Changed behavior of `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup`
  and `MeetingConfig.includeGroupsInChargeDefinedOnCategory`: before values were
  evaluated when asked but this may break old items if `groupsInCharge` changed on
  `proposingGroup` or `category`.
  Now when using these parameters, the values will be stored on the item.
  [gbastien]
- Adapted `MeetingConfig.getItemTypeName` `configType=None` parameter that may
  now accept a value `all`, in this case, all item related types are returned
  (`normal`, `item template`, `recurring item`).
  [gbastien]
- Fixed JS callback `onsuccessManageAttendees` called by `imio.helpers`
  `submitFormHelper` JS function, now received data is an `arraybuffer`,
  no more a `String`.
  [gbastien]
- Added back `Meeting.getSelf` method.
  [gbastien]
- Added helper `ToolPloneMeeting.user_is_in_org(org_id)` that will return `True`
  if a user is in a Plone groups of the given organization id.
  [gbastien]
- Added helper `PloneMeetingTestCase._enable_annex_config` to ease enabling an
  annex related attribute (`confidentiality`, `publishable`, ...).
  [gbastien]
- In `MeetingItem.listCategorie`s, use `natsort.humansorted` instead
  `natsort.realsorted` that behaves better with numbered categories
  (`1 Cat1`, `1.1 Cat1.1`, ...).
  [gbastien]
- Display the `?` icon next to copy groups on the item view in green when copy
  groups have actually access to the item, in classic grey color otherwise.
  [gbastien]
- Added utils.escape utility function # PM-3462 .
  [odelaere]
- Disabled review_sate filter on orgs-searches # PM-3228.
  [odelaere]
- Hide "Contact" action and add action "Documentation iA.Délib" in user action.
  [anuyens]

#### Version 4.2b11 (2021-01-19)

- Added `Annexes` to selectable values of
  `MeetingConfig.itemsNotViewableVisibleFields`. Not viewable annexes will be
  downloadable. For now, `Advices` are still not showable thru this
  functionnality.
  [gbastien]

#### Version 4.2b10 (2021-01-14)

- Fixed `collective.ckeditor` `Z3CFormWidgetSettings` for `DX` to not use a
  `restrictedTraverse` to check if `cke-save` view is available on context or
  it disables `ajax_save` plugin for users that are not `Manager`.
  [gbastien]

#### Version 4.2b9 (2021-01-14)

- Override `PositionTypes` vocabulary from `collective.contact.plonegroup`,
  as our `Directory.position_types` include gender and number
  (like `Director|Directors|Director|Directors` for example), we only display
  the real relevant value (`Director`) depending on person gender.
  Moreover, this fixes `RedefinedSignatoryForm` that was sometime broken if
  dropdown `position_type` contained a very large value.
  [gbastien]
- Fixed JS errors in Console due to `onScrollMeetingView`.
  [gbastien]

#### Version 4.2b8 (2021-01-06)

- Fixed `MeetingItem.is_assembly_field_used`, only evaluate when item is linked
  to a meeting, that broke the item edit form.
  [gbastien]
- While redefining a signatory on an item, add possibility to select a
  `position_type` as label to use for the signature generated in POD templates.
  [gbastien]
- Only call `MeetingItem._check_required_data` when item is about to be
  presented into a meeting, this way previous transitions may be triggered by
  configured process like Webservice call or when item sent from another cfg.
  [gbastien]
- Make the dashboard table header sticky so it is always viewable when
  scrolling, this is the case for every dashboards including
  `available/presented` items on the `meeting_view`.
  [gbastien]
- Enable the `Change ftw labels` batch action on dashboards displaying items.
  To do this, we needed to mark dashboards displaying items and dashboard
  displaying meetings with different batch actions marker interfaces.
  [gbastien]
- Moved `utils.fplog` to `imio.helpers.security`, adapted code accordingly.
  [gbastien]
- As CSS hacks to apply a styling rule only for `Chrome` does not work anymore
  (is taken into account by Firefox as well now), use the `using-chrome`
  CSS class from `plonetheme.imioapps` to style only for Chrome.
  [gbastien]
- `BaseDGHV.printXhtml` `clean` parameter is now `True` by default so it will
  call `separate_images` to avoid several `<img>` in same `<p>`.
  [gbastien]
- When an error occurs on the `MeetingConfig` because of a field in a fieldset
  that is not currently viewable we get a validation error but we do not
  know why.  Display every validation errors at the top of the page so the user
  see what is happening.
  [gbastien]

#### Version 4.2b7 (2020-12-08)

- Use correct icon for `itemfreeze/itempublish` transitions on item workflow
  (were reversed).
  [gbastien]
- Optimized `MeetingItem.updateLocalRoles`, pass `cfg` and `item_state` when
  possible and `ram.cache` for `utils.compute_item_roles_to_assign_to_suffixes`.
  [gbastien]
- Removed `Meeting.items` `ReferenceField`, manage it manually,
  this will help migrating to `DX`.
  [gbastien]
- Do not fail in `vocabularies.PMUsers` when `user_id` contains special chars,
  it may be the case when using `LDAP`, ignore these values.
  [gbastien]
- Optimized `utils.sendMailIfRelevant` to not send an email several times to
  same address.  It was only done in `MeetingItem._sendMailToGroupMembers`.
  Removed `MeetingItem._sendMailToGroupMembers` and manage it using new
  parameter `isGroupIds=True` in `utils.sendMailIfRelevant`.
  [gbastien]
- Make the `quick edit RichText field` work for DX content types :

  - added `PMRichTextWidget` useable in DX schema;
  - renamed `utils.setFieldFromAjax` to `utils.set_field_from_ajax`;
  - migrate `RichTextValue` stored on advices to fix `mimeType/outputMimeType`;
  - moved `MeetingItem._checkMayQuickEdit` to `utils.checkMayQuickEdit` so it
    is easier to reuse;
  - use `PMRichTextWidget` on meetingadvice.

  [gbastien]
- Implement votes functionnality :

  - Added possibility to manage public and secret votes depending
    on MeetingItem.pollType;
  - Added new optional field MeetingItem.votesObservations;
  - Load and manage attendees displayed on item view asynchronously;
  - Use `Products.PloneMeeting.vocabularies.signaturenumbervocabulary`
    everywhere possible and changed from 10 to 20 possible signatories;
  - highlight row in tables to know where we are;
  - Added method for printing votes (print_votes);
  - Refactored the way assembly fields are handled on meeting and item so when
    switching to contacts it behaves correctly when viewing/editing assembly
    fields on old meetings/items.

  [gbastien]
- By default, `searchnotdecidedmeetings` and `searchlastdecisions` Collections
  are displayed chronologically (was reversed before).  No migration applied
  as this may be changed when necessary on Collection itself.
  [gbastien]
- Added parameters `include_hp=False` and `abbreviate_firstname=False` to
  `ItemDocumentGenerationHelperView.print_in_and_out_attendees`.
  [gbastien]
- Fields `committeeObservations` and `votesObservations` are now available on
  both `Meeting` and `MeetingItem`. The `votesObservations` field is only
  writable by `MeetingManagers` and viewable by everybody when meeting or item
  is decided.
  [gbastien]
- When several attendees defined on meeting with same `signature_number`,
  do it correctly useable on items when an signatory is absent.
  When several same `signature_number`, the first present win,
  if not redefined on item, and when redefined, it takes precedence over what
  is defined in meeting.
  [gbastien]
- Completed `MeetingConfig.validate_itemWFValidationLevels` to check, when a
  state is removed, if it is not used by a workflowAdaptation.
  For example workflowAdaptation `waiting_advices` may create state
  `proposed_waiting_advices`, in this case state `proposed` can not be removed
  if some items still in `proposed_waiting_advices`.
  We check every states id beginning with removed states or containing
  `_` + removed state.
  [gbastien]
- Override `@@at_utils` for `IMeetingContent` to fix `Unauthorized` access to
  `@@at_utils` when using `MeetingConfig.itemsNotViewableVisibleFields`
  to show `MeetingItem.category` field.
  [gbastien]

#### Version 4.2b6 (2020-11-19)

- Added parameter `the_objects=False` to `GroupsInChargeVocabulary` and
  `AssociatedGroupsVocabulary` so it is possible to get organization objects as
  term value, this will be used by `plonemeeting.restapi` to return
  `groups_in_charge` and `associated_groups` of a `MeetingConfig`.
  [gbastien]
- Optimized `PloneGroupSettingsValidator` when checking if `plonegroup` used on
  items, do it only if some suffixes removed and use the `portal_catalog`.
- Make sure `attendees` are still editable on item by `MeetingManagers`
  on a decided item if meeting is not closed.
  [gbastien]
- Fixed `MeetingItem._mayClone` that was failing when creating an item from
  a template if `proposingGroup` was defined and `privacy` was `secret`.
  [gbastien]
- Added CompoundCriterion adapters `all-items-to-validate-of-highest-hierarchic-level`
  and `all-items-to-validate-of-every-reviewer-groups` that will return items to
  validate from `normal item validation WF` and
  from `returned_to_proposing_group item validation WF`.
  [gbastien]
- Added email notifications `itemPresentedOwner`, `itemUnpresentedOwner`,
  `itemDelayedOwner` and `returnedToProposingGroupOwner` that notify item
  `Owner` in addition to existing notification `itemPresented`,
  `itemUnpresented`, `itemDelayed` and `returnedToProposingGroup` that notify
  the entire `creators` group.
  In `utils.sendMail`, if event name ends with `Owner` we use mail subject and
  body of corresponding event without the `Owner` suffix.
  [gbastien]
- Completed `Migrate_To_4200._configureItemWFValidationLevels`, migrate fields
  `MeetingConfig.itemAnnexConfidentialVisibleFor`,
  `MeetingConfig.adviceAnnexConfidentialVisibleFor` and
  `MeetingConfig.meetingAnnexConfidentialVisibleFor` that may contain not
  allowed values, but that were not validated in previous version.
  [gbastien]
- Fixed JS form unload protection, that was broken because we redefined
  `window.onbeforeunload`.
  [gbastien]
- Fixed order of CSS (`portal_css`) and JS (`portal_javascripts`) regarding new
  resources (`dexterity.localroles`, `eea.facetednavigation` multiselect widget).
  [gbastien]
- Fixed `Migrate_To_4200._migrateKeepAccessToItemWhenAdviceIsGiven` in case
  attribute `keep_access_to_item_when_advice_is_given` does not exist on
  organization.
  [gbastien]

#### Version 4.2b5 (2020-10-26)

- Do not let `siteadmin` delete a user in production application because,
  that could lead to :

  - losing information (`fullname`) on elements the user interacted with;
  - loading the application and maybe break it as `local_roles` are recomputed
    on every existing elements by Plone when deleting a user.

  [gbastien]

- Fixed adding a MeetingConfig TTW, set correct default values.
  [gbastien]
- Display group `Administrators` members on the MeetingConfig view.
- Manage in and out sentences when attendee was `absent/excused/non attendee`
  from first item. Manage also when attendee is `excused/absent` then
  `non attendee` and so still not present.
  [gbastien]
- Fixed activate correct `portal_tab` while using grouped configs and several
  MC start with same id.
  [gbastien]
- Use position `bottom` to display tooltipster `usersGroupInfos`
  to avoid screen overflow.
  [gbastien]
- Be explicit and always show attendees management icons on the item view,
  was only shown on hover before.
  [gbastien]
- Fixed ploneMeetingSelectItem box (dropdown box for selecting a meeting in the
  plonemeeting portlet) CSS to use light grey background color now that meeting
  state color is kept (was turned to white before).
  [gbastien]
- Changed `MeetingConfig.keepAccessToItemWhenAdviceIsGiven` to
  `MeetingConfig.keepAccessToItemWhenAdvice` so it may handle keeping access to
  item when advice is given or has been giveable.
  [gbastien]
- While using `grouped configs` (dropdown menu in `portal_tabs`), display an
  icon next to the currently selected MeetingConfig.
- Turn `portlet_plonemeeting` label displaying MeetingConfig title into a link
  to the home folder (like the `Home` icon).
  [gbastien]

#### Version 4.2b4 (2020-10-14)

- Make sure `state color` on links is applied everywhere
  (livesearch, livesearch results, folder_contents, ...).
  [gbastien]
- Make sure `events.item_added_or_initialized` is only called one time when
  a new item is created or it may break things done in-between.
  [gbastien]

#### Version 4.2b3 (2020-10-02)

- Added boolean attribute `ConfigurablePODTemplate.store_as_annex_empty_file`,
  when `True`, this will store as annex an empty file instead a generated
  POD template to avoid useless LibreOffice call when stored annex is
  just stored to be replaced by the AMQP process. Moreover when storing as annex
  from the item view, user is no more redirected to the annexes tab, it stays on
  the item view.
  [gbastien]
- Fixed `Migrate_To_4_1._adaptForPlonegroup` to take into account new key
  `enabled` when setting plonegroup functions.
  [gbastien]
- In `imgselectbox` (the box used to select a meeting in the portlet),
  do not append a `/view` to the url of the meeting or it breaks caching because
  by default, other places link to meeting without this `/view`.
  [gbastien]
- Added a new default key displayAdviceReviewState in adaptable method
  `MeetingItem.getCustomAdviceMessageFor` to be able to display advice
  `review_state` to users that may not view the advice.
  [gbastien]
- Fixed link `Go to bottom of the page` on item view for Chrome.
  [gbastien]
- Fixed `@@toggle_item_is_signed` that still reindexed old index
  `getItemIsSigned`, instead new index `item_is_signed`.
  [gbastien]
- Adapted `config.MEETING_GROUP_SUFFIXES` regarding changes in
  `collective.contact.plonegroup`, new key `fct_management` in functions.
  [gbastien]
- Added `held_position.represented_organizations` Relation field to be able to
  specify held_positions representatives of various organizations.
  Moreover, a helper method `organization.get_representatives` is added to get
  representatives held_positions from the organization.
  [gbastien]
- Package `plonemeeting.restapi` is now a direct dependency of `Products.PloneMeeting`.
  [gbastien]
- Added holidays for 2021 and adapted upgrade step to 4200.
  [gbastien]
- Added validation for meeting attendees so it is not possible to unselect an
  attendee if it was redefined on items (itemAbsent, itemExcused,
  itemSignatories, itemNonAttendees).
  [gbastien]
- Added new fields `MeetingItem.decisionEnd`, `MeetingItem.meetingManagersNotesSuite`,
  `MeetingItem.meetingManagersNotesEnd` and
  `MeetingItem.otherMeetingConfigsClonableToFieldDecisionEnd`.
  [gbastien]
- Make `organization.acronym` field viewable/editable also on organizations
  outside `My organization` as it may be used as `associatedGroups` and displayed
  in dashboard in the `Associated groups acronym` column.
  [gbastien]
- Manage down/up WF for some specific advices so icon `waiting_advices_from.png`
  is red when down WF, green when up WF again and blue otherwise.
  [gbastien]
- Refactored `waiting_advices` WFAdaptations to manage more cases.
  [gbastien]
- Added helper `PloneMeetingTestCase.addAdvice`.
  [gbastien]
- Completed `MeetingConfig.validate_itemWFValidationLevels` to not be able to
  disable level if used in the MeetingConfig.
  [gbastien]
- Completed `PloneGroupSettingsValidator` validator, check also composed values
  stored on `MeetingConfig` and using a suffix,
  so values like `suffix_proposing_group_level1reviewers`.
  [gbastien]
- Removed `config.ITEM_STATES_NOT_LINKED_TO_MEETING`, get states in which an item
  is removed from a meeting using `MeetingConfig.itemWFValidationLevels`.
- Setup WFT `default_chain` in `testing.setUpPloneSite` instead `PloneMeetingTestCase.setUp`.
  [gbastien]
- Added parameter `clean=False` to `BaseDGHV.printXhtml` that will use
  `imio.helpers.xhtml.separate_images` to avoid several `<img>` in same `<p>`.
  [gbastien]

#### Version 4.2b2 (2020-09-10)

- Setup more default values for documentenerator.
  [odelaere]
- Added `To discuss?` faceted filter.
  Renamed catalog indexes `getItemIsSigned`, `sendToAuthority` and
  `toDiscuss` to `item_is_signed`, `send_to_authority` and `to_discuss`.
  [gbastien]
- Added CompoundCriterion adapter `items-with-negative-previous-index`, this
  will lookup previous index in the query then negativize defined values.
  [gbastien]
- Added collapsible sections for `budget` and `clonable to other mcs` on item
  view. Added `Toggle show/hide all details action` on the item view to be able
  to toggle every collapsible in one click.
  [gbastien]
- Added an accessor `MeetingItem.getAssociatedGroups` for associatedGroups
  field.
  [aduchene]
- Fixed one security.declarePublic in `MeetingConfig`.
  [aduchene]
- Do not break in `utils.applyOnTransitionFieldTransform` if TAL expression
  does not return a string (especially when it returns `False`).
  [gbastien]
- Refactored item view and edit form to make fields order correspond:

    - order defined on the original item view is used;
    - simple fields (non RichText) are at the top, RichText fields are under;
    - exception for field MeetingItem.otherMeetingConfigsClonableTo, when using
      only simple fields, it is displayed at the top, under
      MeetingItem.sendToAuthority, when using RichText fields
      (otherMeetingConfigsClonableToFieldXXX) it is displayed under the decisions
      fields.

    [gbastien]
- Display field label and fieldset legend a bit larger.
  [gbastien]
- Added parameter `insert_index` to `utils.add_wf_history_action`, this gives
  the possibility to insert a `workflow_history` event at arbitrary position,
  and is used for example when creating an item from `REST WS` and WF
  transitions are triggered, we add event after WF transitions.
  [gbastien]
- Fixed `@@advices-icons` when no advice at all and `Add advice icon` is
  displayed to `power advisers`, the add icon was wrongly styled.
  [gbastien]

#### Version 4.2b1 (2020-08-24)

- Merged changes from 4.1.28
- Added `waiting_advices_from_last_val_level_advices_required_to_validate`
  WFAdaptation to be able to block item validation in case advices still
  need to be given.
- Added adaptable methods `MeetingConfig.extra_item_decided_states` and
  `MeetingConfig.extra_item_positive_decided_states` to formalize how to extend
  `item_decided_states` and `item_positive_decided_states`.
- Added possibility to define data (`title/description/motivation/decision/decisionSuite`)
  to use on an item that will be cloned to another MeetingConfig, data defined on original item
  will replace basic data on resulting item
- Added possibility to configure in `MeetingConfig.itemsVisibleFields` data to display on linked items.
  It is also possible using the `MeetingConfig.itemsNotViewableVisibleFields` and
  `MeetingConfig.itemsNotViewableVisibleFieldsTALExpr` fields to select specific
  data that will be displayed to users that may not access to the linked items
- Workflow adaptations `no_global_observation`, `creator_initiated_decisions` and
  `archiving` were removed as always either enabled or disabled

#### Version 4.2a7 (2020-06-24)

- Merged changes from 4.1.27.1

#### Version 4.2a6 (2020-06-24)

- Merged changes from 4.1.20
- Merged changes from 4.1.21
- Merged changes from 4.1.22
- Merged changes from 4.1.23
- Merged changes from 4.1.24
- Merged changes from 4.1.25
- Merged changes from 4.1.26
- Merged changes from 4.1.26.1
- Merged changes from 4.1.27

#### Version 4.2a5 (2020-03-17)

- Merged changes from 4.1.19.2

#### Version 4.2a4 (2020-03-13)

- Merged changes from 4.1.19

#### Version 4.2a3 (2020-02-21)

- Merged changes from 4.1.18

#### Version 4.2a2 (2020-02-21)

- Merged changes from 4.1.x

#### Version 4.2a1 (2020-02-06)

- Item validation workflow is now designed in the MeetingConfig.itemWFValidationLevels, this imply :
    - to no longer rely on MEETINGROLES and MEETINGREVIEWERS constants;
    - reviewer levels and mapping between review_state and organization suffix that manage the item is computed from the MeetingConfig;
    - item validation specific roles (MeetingMember, MeetingReviewer, MeetingPreReviewer are removed from item workflows, local roles are dynamically given and
      we only use common roles (Reader, Editor, Reviewer and Contributor)
- Use roles 'Reviewer' and 'Contributor' in meetingadvice_workflow
- Added bypass for users having 'Manage portal' in MeetingItemWorkflowConditions in 'mayWait_advices_from', 'mayValidate' and 'mayPresent'

#### Products.MeetingCommunes (4.1.28 → 4.2b1)

#### Version 4.2 (2023-03-06)

- Removed useless import of `get_cachekey_volatile` in `adapters.py`.
  [gbastien]
- Fixed POD template `avis-df.odt` in `examples_fr` profile.
  [gbastien]
- Make `CustomMeetingConfig.getUsedFinanceGroupIds` work with item sent to
  another MC with inheritated advices.
  [gbastien]
- Advices is no more using Plone versioning, removed `repositorytool.xml`
  from `financesadvice` profile (migration is managed by `Products.PloneMeeting`).
  [gbastien]
- Added collection `searchadvicesbacktoitemvalidationstates` using
  `CompoundCriterion` adapter `items-with-advice-back-to-item-validation-states`
  to get items having finances advice that are return in item validation states.
  [gbastien]
- Adapted code regarding removal of `MeetingConfig.useGroupsAsCategories`.
  [gbastien]

#### Version 4.2b24 (2022-09-29)

- Removed wrong ramcache cachekey for `CustomToolPloneMeeting.isFinancialUser`.
  Removed ramcache decorator for it, finally useless.
  [gbastien]

#### Version 4.2b23 (2022-09-22)

- Fixed `examples_fr` profile.
  [gbastien]

#### Version 4.2b22 (2022-08-26)

- Rename "Commission des volontaires" profile to "Bureau des volontaires".
  [aduchene]
- Add helper print method to be able to group by custom method instead of persistent value on item.
  This method must begin by "_group_by_".
  [anuyens, gbastien]
- Field `MeetingConfig.transitionsForPresentingAnItem` was removed, adapted profiles accordingly.
  [gbastien]
- In `MeetingCommunesWorkflowActions.doDecide`, call parent's `doDecide`.
  [gbastien]
- Call migrations to `PloneMeeting 4203 and 4204` in migration to `MeetingCommunes 4200`.
  [gbastien]
- In migration to 4200, removed replace `print_deliberation` by
  `print_full_deliberation` as this last method was removed.
  [gbastien]
- Adapted code now that we use `imio.helpers.cache.get_plone_groups_for_user`
  instead `ToolPloneMeeting.get_plone_groups_for_user`.
  [gbastien]

#### Version 4.2b21 (2022-06-14)

- Add user FS in examples_fr profile.
  [odelaere]
- By default enable the `FINANCE_ADVICES_COLLECTION_ID` collection
  for `meeting-config-zcollege`.
  [gbastien]

#### Version 4.2b20 (2022-05-17)

- Redo release, zest.releaser had set version to 4.2b110...
  [gbastien]

#### Version 4.2b110 (2022-05-17)

- Call migration to `PloneMeeting 4202` in migration to `MeetingCommunes 4200`.
  [gbastien]

#### Version 4.2b19 (2022-05-16)

- Adapt import-csv-inforius.py for MC 4.2.
  [odelaere]
- Fixed `oj-avec-annexes.odt` (`imageOrientation` is now `image_orientation`).
  [gbastien]
- Extended `Migrate_To_4200._adaptWFHistoryForItemsAndMeetings` and renamed it to
  `Migrate_To_4200._adaptWFDataForItemsAndMeetings` as it will also take care to
  migrate `MeetingItem.takenOverByInfos` where the key contains the workflow name.
  [gbastien]
- Do not fail in `CustomMeetingConfig.getUsedFinanceGroupIds` if the collection
  is not enabled, just log a message and return an empty result.
  [gbastien]

#### Version 4.2b18 (2022-04-28)

- Take into account fact that `Migrate_To_4200` may be executed `by parts (a, b, c)`.
  [gbastien]
- Do not redefine `MeetingItemCommunesWorkflowConditions.__init__` as parent
  (`MeetingItemWorkflowConditions`) defines more.
  [gbastien]

#### Version 4.2b17 (2022-03-22)

- Optimized POD template `meeting_assemblies.odt`, use `catalog` available by
  default in the template context instead `self.portal_catalog`.
  [gbastien]
- Call migration to `PloneMeeting 4201` in migration to `MeetingCommunes 4200`.
  [gbastien]

#### Version 4.2b16 (2022-01-07)

- Fixed `MeetingAdviceCommunesWorkflowConditions._check_completeness`, call
  `_is_complete` on the parent (`MeetingItem`).
  [gbastien]

#### Version 4.2b15 (2022-01-03)

- Added two examples in attendees.odt template.
  [aduchene]
- Fixed `council-rapport.odt`, `MeetingItem.listProposingGroups` does not exist anymore.
  [gbastien]

#### Version 4.2b14 (2021-11-26)

- Fixed print_formatted_finance_advice as it was not handling initiative advices properly.
  [aduchene]

#### Version 4.2b13 (2021-11-08)

- Fixed `MCItemDocumentGenerationHelperView.print_all_annexes` to not return
  `</img>` as `<img>` is a self closing tag.
  [gbastien]
- Fixed sample POD templates for meetings to use `view.print_value('date')`
  instead `self.Title()`.
  [gbastien]

#### Version 4.2b12 (2021-10-13)

- In `MCItemDocumentGenerationHelperView.print_creator_name` use
  `ToolPloneMeeting.getUserName` instead `Member.getProperty`.
  [gbastien]

#### Version 4.2b11 (2021-09-09)

- Updated avis-df.odt template to have default value.
  [aduchene]
- Added a `IMeetingCommunesLayer BrowserLayer` so it is possible to override
  PloneMeeting's documentgenerator views without using `overrides.zcml`.
  [gbastien]
- Removed overrided method `CustomMeetingItem._is_complete` as it is the same
  implementation in `Prodducts.PloneMeeting.MeetingItem`.
  [gbastien]

#### Version 4.2b10 (2021-07-16)

- Added new external method to ease the switch to proposingGroupWithGroupInCharge.
  [odelaere]
- Added 2 new profiles `zcodir_extended` and `zcodir_city_cpas`.
  [aduchene]
- Removed default values defined for DashboardCollections `FINANCE_ADVICES_COLLECTION_ID`
  and `searchitemswithnofinanceadvice`, because if it does not exist in the
  `MeetingConfig.customAdvisers`, it breaks the dashboards when applying the profile.
  [gbastien]
- When using finances advice workflows, WF `initial_state` may vary
  (`advicecreated`, `proposed_to_financial_controller`, ...) so when using
  completeness, check that item is complete until the
  `mayProposeToFinancialReviewer` transition guard.
  [gbastien]
- Added `CustomMeetingConfig._setUsedFinanceGroupIds` to ease definition of
  advisers value for the `FINANCE_ADVICES_COLLECTION_ID` collection.
  [gbastien]
- Added PORTAL_CATEGORIES in config.py
  [odelaere]
- Added new listTypes normalnotpublishable and latenotpublishable used in portal.
  [odelaere]
- Adapted `zcity/zcommittee_advice` profiles as advice type `asked_again` is no more optional.
  [gbastien]
- Renamed parameter `listTypes` to `list_types` everywhere.
  [gbastien]
- Moved some methods to snake_case : `printFinanceAdvice/print_finance_advice`,
  `printAllAnnexes/print_all_annexes`, `printFormatedAdvice/print_formated_advice`.
  [gbastien]
- Adapted behavior of `get_grouped_items` with `unrestricted=True` that originally
  returned every items ignoring `itemUids`, it was not possible to print a subset
  of items.  Now if length of `itemUids` is smaller than len of all visible items,
  we only return these items.
  [gbastien]
- Adapted `MCItemDocumentGenerationHelperView.print_item_number_within_category`
  as `MeetingItem.getCategory` does no more return the `proposingGroup` when
  `MeetingConfig.useGroupsAsCategories` is True.
  [gbastien]
- Fixed signature of `MCItemDocumentGenerationHelperView.print_deliberation`.
  [gbastien]
- Added a new DashboardPODTemplate `export-users-groups.ods` in contacts directory.
  [aduchene]
- Improved CustomMeeting.getNumerOfItems using Meeting.getItems.
  [odelaere]
- Improved MCItemDocumentGenerationHelperView.print_all_annexes with filters, icon, better escaping, etc.
  [odelaere]

#### Version 4.2b9 (2021-01-26)

- Added 2 mores formatting examples for `view.print_attendees_by_type` in
  `attendees.odt` template.
  [aduchene]
- Changed uppercases in example_fr profile for `directory_position_types`.
  [aduchene]
- Fixed `MeetingItemCommunesWorkflowActions._doWaitAdvices`, make sure
  `MeetingItem.completeness` is set to `completeness_evaluation_asked_again`
  when advices are asked for the second time (or more).
  [gbastien]
- Adpated code and tests regarding fact that `Meeting` was moved from `AT` to `DX`.
  [gbastien]

#### Version 4.2b8 (2021-01-06)

- Added POD template that renders various votes on item.
  [gbastien]
- Do no more ignore testVotes when executing tests.
  [gbastien]
- Fixed demo profile, items containing annexes were broken because id is
  changed after `categorized_elements` is updated.
  [gbastien]

#### Version 4.2b7 (2020-11-19)

- Fixed a bug in `getPrintableItemsByCategory` (incorrect method call, categories are now in DX).
  [aduchene, gbastien]
- Added `testCustomMeeting.test_GetPrintableItemsByCategoryWithBothLateItems`,
  moved from `Products.MeetingCharleroi`.
  [gbastien]
- Fixed `Migrate_To_4200`, call `addNewSearches` at the end because it needs
  `_adaptWFHistoryForItemsAndMeetings` to have been called in the
  `_after_reinstall` hook to have correct workflows.
  [gbastien]

#### Version 4.2b6 (2020-10-27)

- Added `zcsss` profile to add CSSS MeetingConfig.
  [gbastien]
- Added missing translation for `searchadvicesignedbymanager`.
  [gbastien]

#### Version 4.2b5 (2020-10-14)

- By default use finance `advice_type` for every advice `portal_types`
  that starts with `meetingadvicefinances`.
  [gbastien]

#### Version 4.2b4 (2020-10-02)

- Simplified translation for `MeetingAdviceCommunesWorkflowConditions.mayProposeToFinancialManager`
  `No` message `still_asked_again`.
  [gbastien]
- Fixed `contactsTemplate` dashboard POD template in `examples_fr` profile, set `use_objects=True`.
  [gbastien]
- Added default `directory_position_types` and `contactsTemplates` for `zcpas` profile.
  [gbastien]
- Added translation for `completeness_set_to_not_required_by_app`.
  [gbastien]
- Added collection `searchadvicesignedbymanager` using `CompoundCriterion` adapter
  `items-with-advice-signed-by-financial-manager` to get items having finances advice
  in state `financial_advice_signed`.
  [gbastien]

#### Version 4.2b3 (2020-09-10)

- Fixed `MCMeetingDocumentGenerationHelperView.get_grouped_items` when using
  `excluded_values/included_values` parameters together with `unrestricted=True`,
  unrestricted was not propagated to sub methods giving nonsense results.
  [gbastien]
- Added parameter `additional_catalog_query={}` to
  `MCMeetingDocumentGenerationHelperView.get_grouped_items` making it possible
  to pass additional traditional portal_catalog query to filter items.
  [gbastien]

#### Version 4.2b2 (2020-09-07)

- Added collection `searchitemswithnofinanceadvice` that will use `CompoundCriterion` adapter
  `items-with-negative-previous-index` to get items for which finances advice was not asked.

#### Version 4.2b1 (2020-08-24)

- Added translations for `completeness_not_complete` and `still_asked_again` WF transition button messages.
- Merged changes from 4.1.15
- Adapted profile `zbdc` as `workflowAdaptations` changed.

#### Version 4.2a4 (2020-06-24)

- Merged changes from 4.1.9
- Merged changes from 4.1.10
- Merged changes from 4.1.11
- Merged changes from 4.1.12
- Merged changes from 4.1.13
- Merged changes from 4.1.14

#### Version 4.2a3 (2020-03-13)

- Merged changes from 4.1.8

#### Version 4.2a2 (2020-02-21)

- Merged changes from 4.1.x

#### Version 4.2a1 (2020-02-06)

- Adapted item workflow to use MeetingConfig.itemWFValidationLevels defined configuration
- Added new 'meetingadvice' related workflows : 'meetingadvicefinanceseditor_workflow' and 'meetingadvicefinancesmanager_workflow'
- MeetingConfig.itemDecidedStates and MeetingConfig.itemPositiveDecidedStates fields were removed, adapted import_data files accordingly

#### appy (1.0.8 → 1.0.3)

*No changelog entries found.*

#### imio.annex (2.8 → 2.7)

*No changelog entries found.*

#### imio.helpers (0.47 → 0.31)

*No changelog entries found.*

#### imio.history (1.22 → 1.19)

*No changelog entries found.*

#### imio.prettylink (1.17 → 1.16)

*No changelog entries found.*

#### imio.pyutils (0.22 → 0.11)

*No changelog entries found.*

#### collective.documentgenerator (3.18.1 → 3.18)

*No changelog entries found.*

#### collective.eeafaceted.batchactions (1.6 → 1.5)

*No changelog entries found.*

#### imio.pm.locales (4.1.18.10 → 4.2b1)

#### Version 4.2 (2023-03-06)

- Completed translation `Data that will be used on new item to ${cfg_titles}`.
  [gbastien]
- Do not use `&nbsp;` in committees translations or it is displayed in
  the faceted search filter.
  [gbastien]
- Fixed french translations inversion for `wa_item_validation_shortcuts` and
  `wa_item_validation_no_validate_shortcuts`.
  [gbastien]
- Added translations for `Advice of ${advice_name}`.
  [gbastien]
- Removed unused translation `can_not_remove_attendee_defined_as_signatory`.
  [gbastien]
- Added translation for `title_committees_committee_observations`.
  [gbastien]
- Adapted translation for advice title to include advice label.
  [gbastien]
- Completed translations regarding `committees editors` functionality.
  [gbastien]
- Adapted translations regarding `per vote poll_type` functionality.
  [gbastien]
- Added translations for the `MeetingItem.votesResult` functionality.
  [gbastien]
- Added missing translation for `wa_presented_back_to_wrong_itemWFValidationLevels`.
  [gbastien]
- Added translations regarding `MeetingConfig.itemObserversStates`.
  [gbastien]
- Added trabskations regarding
  WFA `hide_decisions_when_under_writing_check_returned_to_proposing_group`.
  [gbastien]
- Removed translations for field `MeetingConfig.useGroupsAsCategories` that was removed.
  [gbastien]

#### Version 4.2b31 (2022-09-22)

- Added translation for `wa_waiting_advices_given_and_signed_advices_required_to_validate`.
  [gbastien]

#### Version 4.2b30 (2022-09-19)

- Use `"` instead `'` everywhere possible.
  [gbastien]
- For items created from another config, use french term `Créé depuis`
  instead `Reçu depuis`.
  [gbastien]
- Completed attendees changes related translations.
  [gbastien]
- Added translation for `can_not_remove_attendee_defined_as_signatory`.
  [gbastien]

#### Version 4.2b29 (2022-08-26)

- Added translations related to `attendees order by item`.
  [gbastien]
- Removed translations related to field
  `MeetingConfig.transitionsForPresentingAnItem` that was removed.
  [gbastien]
- Added translations related to meeting numbers info and warning messages.
  [gbastien]
- Adapted translations as field `MeetingConfig.yearlyInitMeetingNumber`
  was renamed to `MeetingConfig.yearlyInitMeetingNumbers`.
  [gbastien]
- Added translations related to `item_only` committee.
  [gbastien]
- Adapted `has_required_waiting_advices` to explain to check that
  given advices reached their workflow last step.
  [gbastien]
- Adapted translations for `store_as_annex_type_title` and
  `available_mailing_lists_title` to specify generated format now that
  POD templates are grouped by title in the generationlinks viewlet.
  Added translation for `Please choose a format to generate here next`.
  [gbastien]

#### Version 4.2b28 (2022-07-01)

- Added translations related to `encode votes by group`.
  [gbastien]
- Completed item assembly text related descriptions.
  [gbastien]
- Removed translations for `start_date_before_meeting_date` and
  `end_date_before_meeting_date`.
  [gbastien]

#### Version 4.2b27 (2022-06-14)

- Fixed typos in french for `first_linked_vote_used_vote_values_descr` and
  `next_linked_votes_used_vote_values_descr`.
  [gbastien]
- Added translations for `transfered WF adaptation`.
  [gbastien]

#### Version 4.2b26 (2022-05-10)

- Added translation for `advice_hide_during_redaction_set_auto_to_true`.
  [gbastien]

#### Version 4.2b25 (2022-05-03)

- Completed translation `Item WF validation levels extra suffixes description.`.
  [gbastien]

#### Version 4.2b24 (2022-04-28)

- Added translations for new field `Meeting.adopts_next_agenda_of`.
  [gbastien]
- Added translations for every `levelXreviewers` plonegroup suffixes.
  [gbastien]
- Fixed translation for `can_not_delete_organization_groupsincharge`,
  was `can_not_delete_organization_groupincharge` before (missing `s`).
  [gbastien]
- Added translations for new field `Meeting.mid_start_date`.
  [gbastien]
- Removed `icon_help_waiting_advices_from_xxx` translations, no more used.
  [gbastien]
- Added translation for `proposing_group_with_group_in_charge_required`.
  [gbastien]
- Added translation for `can_not_unselect_plone_group_org`.
  [gbastien]
- Added new WFAdaptations related translations (`dependencies validation`,
  `item_validation_no_validate_shortcuts`, `item_validation_shortcuts`,
  `no_decide`, `no_freeze`).
  [gbastien]
- Added translation for `The configuration does not let you add annexes.`.
  [gbastien]
- Completed translation for `This attendee is marked as ${not_present_type}
  for the ${number} following items (${clusters})`.
  [gbastien]

#### Version 4.2b23 (2022-03-07)

- Added translation `All cache was invalidated`.
  [gbastien]

#### Version 4.2b22 (2022-01-27)

- More generic translation for `internal_notes_descr`.
  [gbastien]

#### Version 4.2b21 (2022-01-21)

- Completed `item_reference_format_descr`.
  [gbastien]

#### Version 4.2b20 (2022-01-14)

- Added help message for column header `header_privacy_help` and
  `header_pollType_help` to get narrower columns.
  [gbastien]

#### Version 4.2b19 (2022-01-14)

- Added translation for `header_async_actions`.
  [gbastien]
- Clarified french translation for `remove_advice_inheritance_ask_locally_not_configured`.
  [gbastien]

#### Version 4.2b18 (2022-01-07)

- Added translation for `Used as item initiator for items`.
  [gbastien]

#### Version 4.2b17 (2022-01-03)

- Added translation for `ckeditor_style_table_optimization`.
  [gbastien]

#### Version 4.2b16 (2022-01-03)

- Added translations for `MeetingConfig.enableAdviceProposingGroupComment`.
  [gbastien]
- Added translation for `listingheader_pod_template_or_odt_file`.
  [gbastien]
- Added translations for `MeetingConfig.itemLabelsEditableByProposingGroupForever`.
  [gbastien]
- Added translations for `MeetingConfig.itemInternalNotesEditableBy`.
  [gbastien]
- Fixed typo in french translation of `PloneMeeting_label_orderedItemInitiators`.
  [gbastien]
- Added translations for `ToolPloneMeeting.deferParentReindex`.
  [gbastien]
- Added translations regarding `Meeting in videoconference` functionality.
  [aduchene]

#### Version 4.2b15 (2021-11-26)

- Small fix in e-mail notification sent when a WF transition is triggered,
  avoid use of `"` in `item_state_changed_default_mail_subject` translation as
  it may also be in translated message leading to `""`.
  [gbastien]
- Make some french translations (`Waiting advices WFA` and `Held position label`)
  more accurate.
  [gbastien]

#### Version 4.2b14 (2021-11-08)

- Added translation for `proposing_group_not_available`.
  [gbastien]
- Added translations regarding `Advice proposing group comment` functionality.
  [gbastien]
- Fixed typo in french translation of `itemDelayed_mail_body`.
  [gbastien]
- Adapted translation for `pod_templates_descr` to include link to
  `Show POD templates details`.
  [gbastien]

#### Version 4.2b13 (2021-09-29)

- More accurate french translation for `can_not_switch_polltype_votes_encoded`.
  [gbastien]

#### Version 4.2b12 (2021-09-28)

- More accurate french translation for `ckeditor_style_pm_anonymize`.
  [gbastien]

#### Version 4.2b11 (2021-09-28)

- Completed french translation for `transition_event_history_aware`.
  [gbastien]
- Added translation for `users_in_suffixed_group` used in
  `MeetingConfig.listSelectableAdvisers` to display number
  of users in advisers Plone group.
  [gbastien]
- Fixed typo in french translation of `PloneMeeting_label_selectableAdviserUsers`.
  [gbastien]
- Completed mail notifications translations `item_state_changed_default_mail_subject`
  and `item_state_changed_default_mail_body` to include transition infos
  (title, actor, comments) now that it is available in received `translationMapping`.
  [gbastien]
- Added translation `ckeditor_style_pm_anonymize`.
  [gbastien]

#### Version 4.2b10 (2021-09-09)

- Added translations for `MeetingConfig.itemPreferredMeetingStates`.
  [aduchene]
- Added translations regarding the `Ask advice to specific users` functionality.
  [gbastien]
- Added translations regarding the `Deadlines to validate items for a meeting` functionality.
  [gbastien]
- Accurate french translations for item navigation widget `Go to next/previous/... item`.
  [gbastien]
- Completed `MeetingConfig.hideHistoryTo` field description.
  [gbastien]
- Adapted translation of field `MeetingCategory.category_id` from `Category identifier`
  to `Category secondary identifier` to avoid confusion with category identifier (id).
  [gbastien]
- Added translations for new mail notification settings.
  [aduchene]
- Completed translations of error messages returned by `MeetingConfig.validate_itemWFValidationLevels`.
  [gbastien]
- Added translations for `MeetingConfig.computeItemReferenceForItemsOutOfMeeting`.
  [gbastien]
- Added translation for `error_some_values_are_not_integers` validation error message.
  [gbastien]

#### Version 4.2b9 (2021-07-16)

- Added translations for `Not completed votes` and `Completed votes`.
  [gbastien]
- Removed single quotes for `meeting_state_changed_default_mail_body`.
  [aduchene]
- Added translations now that `Preferred meeting date` column is abbreviated.
  [gbastien]
- Renamed msgid `You cannot delete the default item template, but you can deactivate it if necessary!` to
  `You cannot delete or move the default item template, but you can deactivate it if necessary!`.
  [gbastien]
- Added translations for `copy_groups_help_msg`.
  [gbastien]
- Adapted translations now that Meeting was moved from AT to DX.
  [gbastien]
- Added translations regarding the `Committees` management.
  [gbastien]
- Changed default translation for `move_item_to_given_position`.
  [gbastien]
- Added translations for annexes faceted filter vocabulary.
  [gbastien]
- Added translation for `required_groupsInCharge_ko`.
  [gbastien]
- Include `item_url` in `holidays_removed_date_in_use_error` translation.
  [gbastien]
- Added translation related to advice behavior that changed (delay no more reinitialized for a given advice).
  [gbastien]
- Removed msgids beginning with `list_type_` in the `PloneMeeting` domain, seem no more used.
  [gbastien]
- Added translations related to `Redefine attendee position on item`.
  [gbastien]
- Changed translation for `no_shown_items` from `No visible item for now.`
  to `You do not have access to these items.`.
  [gbastien]
- Added translation for warning displayed on the meeting view when `assembly/signatures` are not correct.
  [gbastien]
- More accurate translation for `Meeting.meeting_number` and `Meeting.first_item_number`
  description, explaining it is managed by the application.
  [gbastien]
- Added translations for new static columns selectable in `MeetingConfig.meetingColumns`.
  [gbastien]
- Added translations for `not_confidential_annexes`.
  [gbastien]
- Added translations for `Read more/Read less`, removed useless translation
  `This is an extract of the comment, access full comment if necessary...`.
  [gbastien]
- Added translation for `marginal_notes_column`.
  [gbastien]
- Added translation for `not_able_to_find_meeting_to_present_item_into`.
  [gbastien]
- Added translations for `error_default_poll_type_must_be_among_used_poll_types`,
  `error_first_linked_vote_used_vote_values_must_be_among_used_vote_values` and
  `error_next_linked_votes_used_vote_values_must_be_among_used_vote_values`.
  [gbastien]
- Added translation for `title_meetingmanagers_notes`.
  [gbastien]
- Added translation for `MeetingConfig.enabledAnnexesBatchActions`.
  [gbastien]
- Adapted translations for `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup`
  and `MeetingConfig.includeGroupsInChargeDefinedOnCategory` fields description
  now that, when enabled, selected `groupsInCharge` will be stored on the item.
  [gbastien]
- Completed french translation for the help message about copy groups on the item view.
  [gbastien]
- Added translations for `MeetingConfig.selectableRedefinedPositionTypes` and
  `directory.position_types` invariant `removed_redefined_position_type_in_use_error` error message.
  [gbastien]

#### Version 4.2b8 (2021-01-14)

- Accurate french translation for `Position type to use as label for the signature.`.
  [gbastien]

#### Version 4.2b7 (2021-01-06)

- Added translations regarding being able to define a `position_type`
  while redefining a signatory on an item.
  [gbastien]
- Added translation for warning message displayed when an item could not be
  presented using the `@@present-several-items` view.
  [gbastien]
- Added translations for dashboard header title help messages.
  [gbastien]

#### Version 4.2b6 (2020-12-08)

- Reworked `Return to proposing group` related translations.
  [gbastien]
- Added translations for `DX quick edit` related functionality.
  [gbastien]
- Added translations for `votes` functionality.
  [gbastien]
- Added translations for `committeeObservations/votesObservations`
  `Meeting/MeetingItem` fields.
  [gbastien]
- Translate `MeetingCategory` in `PloneMeeting` domain.
  [gbastien]
- Added translation for message displayed on over of redefined
  signatory on meeting or item.
  [gbastien]
- Added translations for MeetingConfig field `itemsVisibleFields`,
  `itemsNotViewableVisibleFields` and `itemsNotViewableVisibleFieldsTALExpr`.
  [gbastien]

#### Version 4.2b5 (2020-11-19)

- Added translations for email notifications `itemPresentedOwner`,
  `itemUnpresentedOwner`, `itemDelayedOwner` and `returnedToProposingGroupOwner`.
  [gbastien]

#### Version 4.2b4 (2020-10-26)

- Better french translation for `only_for_meeting_managers_descr`.
- Adapted translations regarding message displayed in Plone users and groups management
  as we greyed actions Remove user/Remove group.
- Adapted french translation of `meetingconfig_display_groups_and_users_descr`.
- Added translations for `MeetingConfig.keepAccessToItemWhenAdvice` related functionality.
- Added translation for `Currently selected meeting config`.

#### Version 4.2b3 (2020-10-02)

- Added translation for `empty_annex_file_content`.
- Fixed french translations, replace translation `donneur` by `émetteur` everywhere.
- Added translation for `stored_single_item_template_as_annex`.
- Added translations for `held_position.represented_organizations` related functionality.
- Added translations for meeting attendees validation error message.
- Added translations for `waiting_advices` item WF prettylink icon down/up WF.
- Added translations for new fields `MeetingItem.decisionEnd`,
  `MeetingItem.meetingManagersNotesSuite`, `MeetingItem.meetingManagersNotesEnd` and
  `MeetingItem.otherMeetingConfigsClonableToFieldDecisionEnd`.
- Added translations for `waiting_advices` complementary WFAdaptations.

#### Version 4.2b2 (2020-09-10)

- Added translation for `To discuss?` faceted filter.
- Added translations for `To top of the page` and `To bottom of the page`.

#### Version 4.2b1 (2020-08-24)

- Added translation for `has_required_waiting_advices`.
- Merged changes from 4.1.17
- Removed translations for `PloneMeeting_label_itemDecidedStates` and
  `PloneMeeting_label_itemDecidedStates` as corresponding fields were removed
  from MeetingConfig.

#### Version 4.2a5 (2020-06-24)

- Merged changes from 4.1.8
- Merged changes from 4.1.9
- Merged changes from 4.1.10
- Merged changes from 4.1.11
- Merged changes from 4.1.12
- Merged changes from 4.1.13
- Merged changes from 4.1.14
- Merged changes from 4.1.15
- Merged changes from 4.1.16

#### Version 4.2a4 (2020-03-13)

- Merged changes from 4.1.7

#### Version 4.2a3 (2020-02-21)

- Merged changes from 4.1.6

#### Version 4.2a2 (2020-02-21)

- Merged changes from 4.1.5

#### Version 4.2a1 (2020-02-06)

- Adapted translations for mail notification (now that item validation roles are removed, MeetingMember does not exist anymore for example).
- Added translations for default item WF validation levels defined in MeetingConfig.itemWFValidationLevels.
- Added translation for MeetingItem.validate_groupsInCharge error message.

#### imio.pm.ws (2.17 → 2.16)

*No changelog entries found.*

#### plonetheme.imioapps (2.21 → 2.18)

*No changelog entries found.*

## Release 4.1.36

**Date:** 2022-10-20

### Package Updates

#### imio.pyutils (0.11 → 0.22)

#### Version 0.22 (2022-04-28)

- Added `utils.get_clusters` to display a list of number grouped by clusters.
  [gbastien]

#### Version 0.21 (2022-04-26)

- Added `utils.merge_dicts` to be able to merge several dicts for which values
  are list, list are extended in final result.
  [gbastien]

#### Version 0.20 (2022-02-10)

- Modified `memory` to return more useful information.
  [sgeulette]

#### Version 0.19 (2022-01-21)

- Added `process_memory` to return current process memory.
  [sgeulette]
- Added `memory` to return RAM information.
  [sgeulette]

#### Version 0.18 (2022-01-12)

- Made `insert_in_ordereddict` python3 compatible.
  [sgeulette]
- Added `odict_pos_key` to get key at position in ordereddict.
  [sgeulette]

#### Version 0.17 (2022-01-04)

- Added `timed` and `ftimed` functions.
  [sgeulette]
- Added OrderedDict for load_var function
  [sgeulette]

#### Version 0.16 (2021-10-27)

- Added `iterable_as_list_of_list` function.
  [sgeulette]
- Added date in runCommand output
  [sgeulette]

#### Version 0.15 (2021-04-27)

- Added `ln_key` parameter in `read_dictcsv` method.
  [sgeulette]

#### Version 0.14 (2021-04-21)

- Added `read_dictcsv` function.
  [sgeulette]
- Added `utils.replace_in_list` function to ease replacement of values in a list.
  [gbastien]
- Added `safe_encode` function.
  [sgeulette]

#### Version 0.13 (2020-10-07)

- Added `insert_in_ordereddict` function to easier insert a new key at needed position.
  [sgeulette]

#### Version 0.12 (2020-05-19)

- Update syntax for py 3.
  [odelaere]

## Release 4.1.35

**Date:** 2022-04-01

### Package Updates

#### Products.PloneMeeting (4.1.28.34 → 4.1.28.35)

*No changelog entries found.*

## Release 4.1.34

**Date:** 2021-11-09

### Package Updates

#### Products.PloneMeeting (4.1.28.33 → 4.1.28.34)

*No changelog entries found.*

#### imio.pm.ws (2.16 → 2.17)

*No changelog entries found.*

## Release 4.1.33

**Date:** 2021-11-05

### Package Updates

#### Products.PloneMeeting (4.1.28.32 → 4.1.28.33)

*No changelog entries found.*

## Release 4.1.32

**Date:** 2021-11-05

### Package Updates

#### Products.PloneMeeting (4.1.28.31 → 4.1.28.32)

*No changelog entries found.*

## Release 4.1.31

**Date:** 2021-10-28

### Package Updates

#### Products.PloneMeeting (4.1.28.30 → 4.1.28.31)

*No changelog entries found.*

#### imio.helpers (0.46 → 0.47)

#### Version 0.47 (2021-10-13)

- Fixed `content.get_user_fullname` that was breaking when user had no fullname.
  [gbastien]
- Added `content.ur_find` that's the same as api.content.find but unrestrictedly
  [sgeulette]

#### imio.pm.locales (4.1.18.9 → 4.1.18.10)

*No changelog entries found.*

## Release 4.1.30

**Date:** 2021-10-05

### Package Updates

#### Products.PloneMeeting (4.1.28.28 → 4.1.28.30)

*No changelog entries found.*

#### imio.helpers (0.44 → 0.46)

#### Version 0.46 (2021-09-28)

- Added `xhtml.replace_content` function that will replace the content of given
  XHTML tag with some other content. This relies on package `cssselect` that is
  added as an extra dependency thru `imio.helpers[lxml]`.
  [gbastien]

#### Version 0.45 (2021-07-16)

- Added `imio.helpers.SortedUsers`, a vocabulary listing users sorted using
  `natsort.humansorted`. We need to rely on `natsort` to handle this.
  [gbastien]
- Fixed bug in JS function `submitFormHelperOnsuccessDefault` called onsuccess
  by `submitFormHelper` to only consider response as a file to return if
  responser header `content-length` is found in request, this avoid returning
  a wrong blob object when called code returns an error message.
  [gbastien]

#### imio.pm.locales (4.1.18.8 → 4.1.18.9)

*No changelog entries found.*

## Release 4.1.29

**Date:** 2021-09-08

### Package Updates

#### appy (1.0.6 → 1.0.8)

*No changelog entries found.*

## Release 4.1.28

**Date:** 2021-08-17

### Package Updates

#### Products.PloneMeeting (4.1.28.27 → 4.1.28.28)

*No changelog entries found.*

#### Products.MeetingCommunes (4.1.27 → 4.1.28)

*No changelog entries found.*

## Release 4.1.27

**Date:** 2021-07-26

### Package Updates

#### imio.helpers (0.43 → 0.44)

#### Version 0.44 (2021-06-15)

- In `xhtml.separate_images` be a bit less defensive, too complex cases are
  still ignored but when the `<p>` contains only non textual elements like
  `<br>` or `blanks`, just ignore these elements.
  [gbastien]

## Release 4.1.26

**Date:** 2021-05-31

### Package Updates

#### Products.PloneMeeting (4.1.28.26 → 4.1.28.27)

*No changelog entries found.*

#### Products.MeetingCommunes (4.1.26 → 4.1.27)

*No changelog entries found.*

#### imio.helpers (0.40 → 0.43)

#### Version 0.43 (2021-05-31)

- Lowercased email address after validation.
  [sgeulette]
- Fixed `submitFormHelperOnsuccessDefault` JS function to handle binary response
  so it is possible to download the result of the ajax query.
- Added `xhtml.imagesToData` that turns the src of images used in a xhtml
  content from an `http` or equivalent URL to a data base64 value.
  [gbastien]

#### Version 0.42 (2021-04-30)

- Added parameter `filetype='PNG'` to `barcode.generate_barcode` so it is
  possible to use another supported image file format.
  [gbastien]
- Added parameter `replyto` to `emailer.send_email` so it is possible to add
  `reply-to` header in message
  [sgeulette]
- Adapted `content.object_values` and `content.object_ids` to be able to pass
  a single class name or a list of class names like it is the case for
  `objectValues/objectIds`.
  [gbastien]

#### Version 0.41 (2021-04-21)

- Corrected encoding problem in emailer.
  [sgeulette]

#### imio.pm.locales (4.1.18.7 → 4.1.18.8)

*No changelog entries found.*

## Release 4.1.25

**Date:** 2021-05-27

### Package Updates

#### Products.PloneMeeting (4.1.28.25 → 4.1.28.26)

*No changelog entries found.*

#### Products.MeetingCommunes (4.1.25 → 4.1.26)

*No changelog entries found.*

#### collective.documentgenerator (3.18 → 3.18.1)

*No changelog entries found.*

#### imio.pm.locales (4.1.18.6 → 4.1.18.7)

*No changelog entries found.*

## Release 4.1.24

**Date:** 2021-04-28

### Package Updates

#### Products.PloneMeeting (4.1.28.21 → 4.1.28.25)

*No changelog entries found.*

#### Products.MeetingCommunes (4.1.23 → 4.1.25)

*No changelog entries found.*

#### imio.annex (2.7 → 2.8)

#### Version 2.8 (2021-04-23)

- Fixed `quickupload.ImioAnnexQuickUploadCapableFileFactory` to make sure that
  thread lock is released like it is the case by default in
  `uploadcapable.QuickUploadCapableFileFactory`.
  This should avoid rare cases where instance is stuck while adding an annex.
  [gbastien]

## Release 4.1.24-seraing

**Date:** 2021-04-07

### Package Updates

#### Products.PloneMeeting (4.1.28.18 → 4.1.28.21)

*No changelog entries found.*

#### Products.MeetingCommunes (4.1.21 → 4.1.23)

*No changelog entries found.*

#### appy (1.0.5 → 1.0.6)

*No changelog entries found.*

#### imio.helpers (0.37 → 0.40)

#### Version 0.40 (2021-04-01)

- Added `target` option in `object_link` function
  [sgeulette]
- Added a ZPublisher `:json` suffix type converter.
  [gbastien]
- Changed MockMailHost patch to avoid some problems
  [sgeulette]
- Make `xhtml.storeImagesLocally` handle images with `src` using base64 encoded
  data (like `data:image/png;base64,...)`.
  [gbastien]

#### Version 0.39 (2021-02-25)

- Added `validate_email_address` to check email address with a real name part.
  [sgeulette]
- Added `validate_email_addresses` to check email addresses, separated by a comma.
  [sgeulette]
- Added `content.get_modified_attrs`, when called in a `IObjectModifiedEvent`
  handler, will return the list of field names that were actually modified.
  [gbastien]
- Returned email sender error messages.
  [sgeulette]
- Added `content.uuidToCatalogBrain` that is a shortcut to
  `content.uuidsToCatalogBrains` but that will return a single value.
  [gbastien]
- Added `content.object_values` and `content.object_ids` method, equivalent to
  Zope's `objectValues` and `objectIds` but that will check contained element
  class name instead `meta_type` so it works with DX content types where
  `meta_type` is the same for every types.
  [gbastien]
- Added `content.uuidToObject` that is a shortcut to
  `content.uuidsToObjects` but that will return a single value.
  [gbastien]
- Corrected `has_faceted` function call in `submitFormHelperOnsuccessDefault` js
  [sgeulette]
- Reloaded page when `submitFormHelper` is used on a non faceted page
  [sgeulette]
- Added parameter `toggle_type='slide'` to JS helper `toggleDetails`,
  so it is possible to use `slideToggle` (default) or `fadeToggle`.
  `fadeToggle` behaves better when the hidden part contains a sticky element
  (table header).
  [gbastien]

#### Version 0.38 (2021-01-06)

- Added `content.normalize_name` that will normalize a given name, this is the
  code used when turning a title to an id when creating a new content.
  [gbastien]

#### imio.history (1.20 → 1.22)

#### Version 1.22 (2021-03-04)

- Changed default to `False` for parameters `checkMayViewEvent=False` and
  `checkMayViewComment=False` of `utils.getLastAction`, this way, we get last
  action even if current user may not, and it is quicker.
  This fix a performance issue in `ImioWfHistoryAdapter.historyLastEventHasComments`
  when called several times.
  [gbastien]
- In `utils.getLastAction`, parameter `action` may be `before_last` and will
  return the before last action if it exists.
  [gbastien]

#### Version 1.21 (2020-10-26)

- Added helper `utils.get_all_history_attr` to get every occurence of a given
  `attr_name` in a `history`. This will return every `review_state` from the
  `workflow` history for example.
  [gbastien]

#### imio.pm.locales (4.1.18.3 → 4.1.18.6)

*No changelog entries found.*

## Release 4.1.23

**Date:** 2021-02-12

### Package Updates

#### Products.PloneMeeting (4.1.28.17 → 4.1.28.18)

*No changelog entries found.*

#### Products.MeetingCommunes (4.1.20 → 4.1.21)

*No changelog entries found.*

#### appy (1.0.4 → 1.0.5)

*No changelog entries found.*

## Release 4.1.22

**Date:** 2021-01-26

### Package Updates

#### Products.PloneMeeting (4.1.28.15 → 4.1.28.17)

*No changelog entries found.*

#### imio.helpers (0.35 → 0.37)

#### Version 0.37 (2020-12-21)

- Added JS function `submitFormHelper` that will submit a given form and
  `onsuccess`, will call the function `onsuccess` in parameter
  (by default, when called in an overlay, will close the overlay and
  reload the faceted navigation).
  [gbastien]
- Added `security.fplog` helper to ease adding a `collective.fingerpointing`
  message to the log.
  [gbastien]
- Added `plone.app.relationfield` as a direct dependency.
  [gbastien]

#### Version 0.36 (2020-12-07)

- Added email functions (`create_html_email`, `add_attachment`, `send_email`)
  to create and send an email with attachments.
  [sgeulette]
- Optimized `xhtml.separate_images`, do only walk the tree if
  it contains images (`img` tag).
  [gbastien]
- Fixed `content.richtextval` `outputMimeType` parameter to use
  `text/x-html-safe` instead `text/html`.
  [gbastien]
- Renamed JS function `loadCollapsibleContent` to `loadContent` as it can be
  used outside of `collapsible` scope.
  [gbastien]

#### collective.eeafaceted.batchactions (1.5 → 1.6)

#### Version 1.6 (2020-12-21)

- After action applied, do not reload the entire page,
  just reload the current faceted results.
  [gbastien]
- Use `CheckBoxFieldWidget` instead `SelectFieldWidget` to manage labels to
  (un)select in `LabelsBatchActionForm` to avoid manipulation with
  `CTRL+click` for selection. Adapted and rationalized translations.
  [gbastien]
- Add a `collective.fingerpointing` entry when applying action to know
  which action was applied on how much elements.
  [gbastien]

#### imio.pm.locales (4.1.18.2 → 4.1.18.3)

*No changelog entries found.*

#### plonetheme.imioapps (2.19 → 2.21)

#### Version 2.21 (2020-10-07)

- imioapps : skin data displayed in `PrettyLinkWithAdditionalInfosColumn` column,
  add some margin between data.
  [gbastien]

#### Version 2.20 (2020-09-07)

- plonemeetingskin : increase base line-height as font-size was increased.
  [gbastien]

## Release 4.1.21

**Date:** 2020-11-24

### Package Updates

#### Products.PloneMeeting (4.1.28.2 → 4.1.28.15)

*No changelog entries found.*

#### Products.MeetingCommunes (4.1.15 → 4.1.20)

*No changelog entries found.*

#### appy (1.0.3 → 1.0.4)

*No changelog entries found.*

#### imio.helpers (0.31 → 0.35)

#### Version 0.35 (2020-11-18)

- Added JS helper method `canonical_url` to get the current canonical URL
  so the url of the context when on a view.
  [gbastien]
- In `toggleDetails` JS function, moved the part that does the async load in
  `loadCollapsibleContent` function so it is possible to call if from outside.
  [gbastien]
- Added `get_user_from_criteria` helper method to search users following
  email or fullname
  [sgeulette]
- Added param on `transitions` method, to not warn by default
  [sgeulette]
- Completed `appy_pod` usecases, `font-size 50%/150%`.
  [gbastien]
- Added `catalog.merge_queries` function that merges `plone.app.querystring`
  compatible catalog queries into one single query.
  [gbastien]
- Do not break in `xhtml.storeImagesLocally` if a `NotFound` occurs while
  getting an internal image.
  [gbastien]

#### Version 0.34 (2020-10-16)

- Moved JS function `setoddeven` from `listings.js` to
  `helpers.js` so it is available by default.
  [gbastien]
- Added setup_logger in security module to change logger level (when
  doing `instance run` by example)
  [sgeulette]

#### Version 0.33 (2020-10-01)

- Added `content.get_relations` and `content.get_back_relations` to easily
  get relations and back relations on an object.
  [gbastien]
- Do not break in `xhtml.storeImagesLocally` if image URL
  contains non-ASCII characters.
  [gbastien]
- Added `xhtml.separate_images` that will make sure images are separated in
  different `<p>` to avoid breaking `appy.pod` when using `LibreOffice 6.0.x`.
  [gbastien]

#### Version 0.32 (2020-09-10)

- Log every 1000 elements instead 100 in `catalog.addOrUpdateIndexes` and
  `catalog.reindexIndexes`.
  [gbastien]
- Fixed code to make except Exception syntax Python 3.8 compatible.
  [gbastien]

#### imio.history (1.19 → 1.20)

#### Version 1.20 (2020-10-01)

- Added parameters `checkMayViewEvent=False` and `checkMayViewComment=False` to
  `utils.getLastWFAction`, this way, we get last WF action even if current user
  may not, and it is quicker.
  [gbastien]

#### imio.prettylink (1.16 → 1.17)

#### Version 1.17 (2020-10-06)

- Set icons `<img>` tag `width=16px` and `height=16px` to make `tooltipster`
  happy (computed area to display depends on displayed content).
  [gbaastien]

#### imio.pm.locales (4.1.17 → 4.1.18.2)

*No changelog entries found.*

## Release 4.1.20

**Date:** 2020-09-03

### Package Updates

#### Products.PloneMeeting (4.1.27.2 → 4.1.28.2)

#### Version 4.1.28.1 (2020-08-21)

- When getting a `position_type_attr` on a `held_position.get_label`, added possibility to fallback to another `position_type_attr`
  if given one is empty.  This makes it possible to fallback to `position_type` while trying to get `secondary_position_type`
  and this last is empty
- Hide button `Add group` in Plone groups configuration panel with CSS, this avoid users to add Plone groups instead organizations

#### Version 4.1.28 (2020-08-21)

- Moved `Meeting.getNextMeeting` logic to `utils.get_next_meeting` so it can be used from outside a `Meeting` instance,
  moreover, make negative `dateGap` work, this is useful to get `Meeting` of today when meeting have no hours defined
- Make sure the faceted ajax spinner is visible when loading available items on a meeting or page seems somewhat stucked
- A `MeetingConfig` used in another `MeetingConfig.meetingConfigsToCloneTo` can not be deactivated
- When CSS style `border:none;` on a table, no matter border on cells are defined, tables rendered by `appy.pod`
  do not have a border, so displaying it as dotted border in `CKeditor`
- In `@@display-group-users`, if group contains another group, display group's title instead group id (or group id if no title),
  moreover clearly differenciate using `user.png/group.png` icon when member is a user or a group
- Enabled column `PloneGroupUsersGroupsColumn` on contacts dashboard displaying organizations
- Enabled `allow_reorder` for `organization.certified_signatures` DataGridField
- Use `ram.cache` for `SelectableAssemblyMembersVocabulary` used in `organization.certified_signatures` DataGridField
  so it renders faster in dashboards displaying organizations
- Make `organization`/`person`/`held_position` implements `IConfigElement` so we may use `_invalidateCachedVocabularies`
  to invalidate cached vocabularies and it is not necessary to write event handlers for these cases
- Added `group-users` icon next to `proposingGroup` to display every Plone groups members to members of the `proposingGroup` only
- Added `collective.fingerpointing` log message when managing item `assembly/signatures/attendees/signatories`
- Fixed bug in `itemPeople` macro displayed on `meetingitem_view`, when field Meeting `itemNonAttendees` is enabled,
  the column header was correctly hidden but the column cells were displayed
- Moved JS function `toggleDoc` to `imio.helpers` under name `toggleDetails`
- Cleaned `plonemeeting.css`, removed useless styles definition
- In `contacts` management, show clearly that icons in portlet will add new `organization/held_position` by using icons with a `+`
- Validate `plonegroup` settings for `functions` so it is not possible to remove or disable a function that is used in
  `MeetingConfig.selectableCopyGroups` or `MeetingItem.copyGroups`
- Migrate `MeetingCategory` from AT to DX :

  - New portal_type is `meetingcategory`;
  - Field `MeetingItem.classifier` was moved from ReferenceField to StringField;
  - Added new `MeetingConfig.insertingMethodsOnAddItem` named `on_classifiers`;
  - Removed magic in `MeetingConfig.getCategories` that returned organizations when
    `MeetingConfig.useGroupsAsCategories` was `True`, now it returns only categories, moreover parameter `classifiers` is
    renamed to `catType` that may be `all`/`categories`/`classifiers`.
- In every migrations, call `cleanRegistries` at the end by default so `JS/CSS` are recompiled
- Add 'redirectToNextMeeting' option.
- Moved `Meeting.getNextMeeting` logic to `utils.get_next_meeting` so it can be used from outside a `Meeting` instance
- Make sure `++resource++plone.app.jquerytools.dateinput.js` is enabled in `portal_javascripts`
- Completed custom widget `PMCheckBoxFieldWidget` to manage `display` mode, every element are listed one under each other and not one
  next to each others separated with commas that was much unreadable when having more than 3 values.
  Use it everywhere possible: `organization`, `held_position` and `category`
- Fixed `MeetingView._displayAvailableItemsTo`, do not use `ToolPloneMeeting.userIsAmong` for powerobservers as it could be
  powerobserver for `MeetingConfig` A and not for `MeetingConfig` B and in this case, the available items were shown
- Added `CKEditor` style `page-break` to be able to insert a `page-break` into a `RichText` field, this can be used in a
  `POD template` by adding a relevant `page-break` paragraph style
- In `MeetingItemWorkflowConditions._check_review_and_required`, factorized check about `Review portal content` permission and
  required data (`category/classifier/groupsInCharge`)
- Improved `BaseDGHV.print_signatories_by_position` to add more use cases
- Added tests for `BaseDGHV.print_signatories_by_position`
- Adapted code regarding changes in `collective.iconifiedcategory`, do not use `portal_catalog` to get the annexes but rely on
  `allowedRolesAndUsers` stored in `categorized_elements`
- Fixed `MeetingView._displayAvailableItemsTo`, do not use `ToolPloneMeeting.userIsAmong` for powerobservers as it could be
  powerobserver for `MeetingConfig` A and not for `MeetingConfig` B and in this case, the available items were shown
- Display groups created by a `MeetingConfig` (meetingmanagers, powerobservers, ...) on the `meetingconfig_view`.
  Moved the `@@display-group-users` view to `collective.contact.plonegroup` so we have same view to render groups and users in
  contacts dashboard and everywhere else.
- Extended batch action that stores a generated template directly as an annex on selected elements.
  Field `MeetingConfig.meetingItemTemplateToStoreAsAnnex` is now `MeetingConfig.meetingItemTemplatesToStoreAsAnnex` and several
  POD templates may be selected instead one single.  In the batch action, the user may chose among available POD templates
- Fixed `@@check-pod-templates` that was no more raising an error when a POD template was wrong, hidding broken templates...
- Reworked email notifications to always have relevant information at the beginning of the subject in case item title is very long
- Make sure field `Meeting.secretMeetingObservations` is only editable/viewable by `MeetingManagers`

#### Products.MeetingCommunes (4.1.14 → 4.1.15)

#### Version 4.1.15 (2020-08-21)

- Fix translations for `MeetingExecutive`.
  [vpiret]
- Add BDC Profiles
  [anuyens]
- Add missing translations for MeetingAudit.
  [anuyens]
- Added translations for actions `sent to` from `College/BP` to `CoDir`.
  [gbastien]
- Define style `page-break` in `deliberation.odt` POD template.
  [gbastien]
- Added more `position_types` by default (secretaire) in `examples_fr` profile.
  [gbastien]

#### imio.actionspanel (1.49 → 1.50)

#### Version 1.50 (2020-08-18)

- Make CSS rule for `input[type="button"].notTriggerableTransitionButton` more
  specific so it is taken into account.
  [gbastien]
- Fix message (tag title) displayed on a not triggerable WF transition when
  displayed as a button, the transition title was not included in the message.
  [gbastien]

#### imio.dashboard (2.7 → 2.8)

#### Version 2.8 (2020-08-18)

- Enable `PloneGroupUsersGroupsColumn` in dashboards displaying organizations.
  [gbastien]

#### imio.helpers (0.30 → 0.31)

#### Version 0.31 (2020-08-18)

- Correctly translate a utf8 state title.
  [sgeulette]
- Added `content.safe_delattr` to avoid having to check `base_hasattr` before.
  [gbastien]
- Added JS helper function `toggleDetails` to be able to show/hide details
  using a collapsable `<div>`.
  [gbastien]
- Completed `appy_pod` usecases,
  fixed images to use https://picsum.photos/ instead https://www.imio.be
  [gbastien]

#### imio.migrator (1.23 → 1.25)

#### Version 1.25 (2020-08-18)

- In `Migrator.removeUnusedPortalTypes`, remove also `portal_types` from
  `site_properties.types_not_searched`.
  [gbastien]

#### Version 1.24 (2020-06-29)

- Fix python 3.8 synthax error.
  [odelaere]

#### collective.contact.core (1.32 → 1.33)

#### Version 1.33 (2020-08-18)

- Add new `enterprise number` field for organization content type
  [laulaz]
- Updated Title to work with transmogrifier
  [sgeulette]
- Updated birthday widget to manage dates range
  [sgeulette]
- Added `create_organization.png` icon useable if necessary
  [gbastien]

#### collective.contact.plonegroup (1.28 → 1.29.1)

#### Version 1.29.1 (2020-08-26)

- Fix CSS for `@@display-group-users` view when current user not a Manager
  and so does not have link on prefixed icon (user/group).
  [gbastien]

#### Version 1.29 (2020-08-18)

- Added `PloneGroupUsersGroupsColumn`, a column that displays suffixed groups
  and users, to be called on dashboard displaying organizations.
  The groups and users are rendered by the `@@display-group-users` view
  that may also be used outside.
  By default, as groups and users may be very long to display, it is hidden
  in a collapsible `<div>` and displayed asynchronously.
  [gbastien]
- Added possibility to disable a `function` (`enabled=True` by default),
  this is useful to avoid deleting a `function` and re-adding it after,
  sometimes faultly.  Adapted `utils.get_all_suffixes(only_enabled=True)`
  to only get enabled functions.
  Added upgrade step to version `6` to manage new value `enabled=True`
  in `functions` stored in the `regsitry`.
  [gbastien]
- Remove item `UID` from link in `OrgaPrettyLinkWithAdditionalInfosColumn`
  as it is now displayed as additional information by default.
  [gbastien]

#### collective.documentgenerator (3.17 → 3.18)

#### Version 3.18 (2020-08-18)

- Updated file_representation to be compliant with zopeedit < 1.0 (current windows exe) and zopeedit >= 1.0.
  [sgeulette]
- Fixed bug when rendering an empty RichTextATFieldRenderer.
  [odelaere]
- Pass `kwargs` given to `DocumentGenerationView.__call__`,
  to submethods `generate_and_download_doc`,  `_generate_doc`,
  `_recursive_generate_doc` then `_render_document` so it is possible to pass
  `raiseOnError=False` parameter to `_render_document`.
  [gbastien]

#### collective.eeafaceted.dashboard (0.13.1 → 0.13.2)

#### Version 0.13.2 (2020-08-18)

- Fixed IndexError when generating a dashboardpotemplte whith empty elements.
  [odelaere]

#### collective.eeafaceted.z3ctable (2.10 → 2.11)

#### Version 2.11 (2020-08-18)

- Render `DataGridField` in `PrettyLinkWithAdditionalInfosColumn` vertically.
  [gbastien]
- Bugfix in `PrettyLinkWithAdditionalInfosColumn`, sometimes the widget's
  context was the previous row object.
  [gbastien]
- Added parameter `PrettyLinkWithAdditionalInfosColumn.simplified_datagridfield`
  and set it to `False` by default.
  [gbastien]
- Moved `MemberIdColumn.get_user_fullname` out of `MemberIdColumn` so it can be
  easily used from outside.
  [gbastien]
- Added `PrettyLinkWithAdditionalInfosColumn.ai_extra_fields`, that
  let's include extra data not present in schema, by default this will include
  `id`, `UID` and `description`.
  [gbastien]

#### collective.iconifiedcategory (0.46 → 0.47)

#### Version 0.47 (2020-08-18)

- Added missing translation for `Nothing.`.
  [gbastien]
- In `utils._categorized_elements`, use `aq_base` to get `categorized_elements`
  to be sure we get the one on context.
  Indeed the parent could have this attribute too...
  [gbastien]
- Do not use `portal_catalog` to get `categorized_elements`, instead, store
  `allowedRolesAndUsers` in the `categorized_elements` data and rely on it to
  get the content directly stored in the parent.  This for performance reasons.
  [gbastien]
- Remove unused `utils.get_UID` function.
  [gbastien]
- Make sure a content created with an unexisting `content_category`
  does not break anything.
  [gbastien]

#### collective.messagesviewlet (0.21 → 0.23)

#### Version 0.23 (2020-04-17)

- Fix tests & travis build (#8)
  [laulaz]
- Prevent a bug when compare 2 dates with different timezone format.
  [boulch]

#### Version 0.22 (2020-01-15)

- Fix bug when message configuration don't permit to hide this message (close button stayed).
  [boulch]
- Adapted code for Plone5.2/Py3.
  [gbastien]

#### imio.pm.locales (4.1.16 → 4.1.17)

#### Version 4.1.17 (2020-08-21)

- Added translation for `Enabled?`.
- Added translation for warning message explaining why a `MeetingConfig` can not be disabled.
- Added translation for `Data that will be used on new item`.
- Renamed msgid `PloneMeeting_label_categoryMappingsWhenCloningToOtherMC` to
  `PloneMeeting_label_category_mapping_when_cloning_to_other_mc`.
- Adapted `MeetingItem.classifier` related translations.
- Shorter translation for `Signature number` in `DataGridField`, now default is `Number`.
- Added translation for `Items have been reordered.`
- Added translation for `ckeditor_style_page_break`.
- Added translation for `redirectToNextMeeting` option.
- Added translation for `meetingconfig_display_groups_and_users_descr`.
- Removed translation for `no_users_in_group` that was moved to `collective.contact.plonegroup`.
- Removed translation for `View linked Plone groups` that was moved to `collective.contact.plonegroup`.
- Added translation for `POD template to annex`.
- Adapted translations for `MeetingConfig.meetingItemTemplatesToStoreAsAnnex`.
- Reworked email notifications subject to always have relevant information at
  the beginning of the subject in case item title is very long.
- Rationalized every field descr using translation `only editable/vieable by MeetingManagers` and
  `only editable by MeetingManagers but viewable by everyone`.
- Added more accurate translation for `warning_adding_org_outside_own_org`.

#### plonetheme.imioapps (2.17 → 2.19)

#### Version 2.19 (2020-09-01)

- Fix input text/passowrd and textarea background-color so default styles
  applied by Firefox are overrided (Firefox 80+).
  [gbastien]

#### Version 2.18 (2020-08-18)

- imioapps : style the `PloneGroupUsersGroupsColumn` column.
  [gbastien]
- plonemeetingskin : make sure very large images are not
  exceeding the screen.
  [gbastien]
- plonemeetingskin : removed useless styles about `actionMenuAX`
  that was replaced by `tooltipster`.
  [gbastien]
- imioapps : make sure input submit/button use `cursor:pointer`, moreover
  fix Firefox disappearance of `outline` when an `input submit` is clicked,
  replace it with a `box-shadow` as we use `border-radius`.
  [gbastien]
- imioapps : remove multiple definition for `#content legend padding`.
  [gbastien]

## Release 4.1.19.1

**Date:** 2020-09-08

### Package Updates

#### appy (0.9.16 → 1.0.3)

*No changelog entries found.*

## Release 4.1.19

**Date:** 2020-06-25

### Package Updates

#### Products.PloneMeeting (4.1.25.1 → 4.1.27.2)

#### Version 4.1.27.2 (2020-06-25)

- Adapted `CheckPodTemplatesView` so generation helper view is correctly initialized when generating pod template on meeting,
  this would have shown the `max_objects` bug in `collective.eeafaceted.dashboard` `_get_generation_context` method
- Force email sender address in upgrade step to 4109

#### Version 4.1.27.1 (2020-06-24)

- In `MeetingItem.getAdviceDataFor`, hide also `observations`, like it is already the case for `comment`' when
  `hide_advices_under_redaction=True` and advice is currently under redaction

#### Version 4.1.27 (2020-06-24)

- Fixed bug in `DashboardCollection` stored `query`, instead list of `<dict>`, was sometimes list of `<instance>`
  (???), added upgrade step to 4108, this is necessary for `plone.restapi` to serialize `DashboardCollection` to json
- Fixed wrong `TAL condition` used for `DashboardCollection` `searchmyitemstakenover` (replaced `omittedSuffixed` by `omitted_suffixes`)
- Added parameter `ignore_underscore=False` to `utils.org_id_to_uid`, when an underscore is present, the value is considered
  something like `developers_creators`, if it is actually an organization id containing an `_` (which is not possible by default),
  then set `ignore_underscore=True` to get it.
- Display `groupsInCharge` on the item view : when field `MeetingItem.groupsInCharge` is used, from the proposingGroup when
  `MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup=True` or from the category when
  `MeetingConfig.includeGroupsInChargeDefinedOnCategory=True`.
  Set `autoInclude=True` by default instead `False` for `MeetingItem.getGroupsInCharge`
- Fix `email_from_address` in migration 4108 so it is unique for each customers and helps to lower the spam score.
- Set `MeetingItem.getGroupsInCharge(autoInclude=True)` by default instead `autoInclude=False` so calling the accessor without parameter
  returns `groupsInCharge` stored on `proposingGroup` or `category`
- Display `DashboardCollection` UID on the `MeetingConfig` view
- When cloning item to another `MeetingConfig`, keep `copyGroups` by default
  (`copyGroups` moved from `config.EXTRA_COPIED_FIELDS_SAME_MC` to `config.DEFAULT_COPIED_FIELDS`)
- Factorized check about required data to be able to trigger a transition on an item in `MeetingItemWorkflowConditions._check_required_data`,
  this way we check if `category/groupsInCharge` are correct
- Added `collective.fingerpointing` log message when using `ToolPloneMeeting.updateAllLocalRoles` so we know who and how much
- Simplified `Meeting.getRawQuery` to only use `linkedMeetingUID` index to query items,
  remove useless index `portal_type` from query as `linkedMeetingUID` is sure to be unique
- Adapted override of `generationlinks.pt` regarding changes in `collective.eeafaceted.dashboard` (`pod_template.max_objects` attribute)
- Validate `directory.position_types` to check that a used `position_type` (by a `held_position`) can not be removed

#### Version 4.1.26.1 (2020-06-12)

- Reworked `wait_advices_from.png` so it is correctly displayed with a background
- Search plone groups based on org UID instead of title to avoid mismatch.
  [odelaere]
- Fix `Migrate_To_4105`, call to `upgradeAll` should always omit profiles `Products.PloneMeeting` and `self.profile_name`
- Display `DashboardCollection` id next to title on `MeetingConfig` view

#### Version 4.1.26 (2020-06-11)

- Use `Products.Archetypes.interfaces.IObjectInitializedEvent` and `zope.lifecycleevent.interfaces.IObjectAddedEvent`
  to initialize freshly created item to make `plone.restapi` happy or item is not initialized and attributes
  like `adviceIndex` are not added.  With `plone.restapi`, validation is done after `ObjectInitializedEvent` but before `ObjectAddedEvent`.
  Implement also `MeetingItem.initializeArchetype` in which we call `events.item_added_or_initialized` or
  some fields are not writable for `plone.restapi` because `MeetingMember` role is not given...
- Added missing icon `wait_advices_from.png`
- Do not fail in `vocabularies.PMCategoryVocabulary` when creating an annex using `plone.restapi`,
  validation is done before annex is fully initialized
- Set `enforceVocabulary=True` for `MeetingItem.proposingGroup`, `MeetingItem.proposingGroupWithGroupInCharge`, `MeetingItem.groupsInCharge`
  and `MeetingItem.optionalAdvisers` so validation is done correctly when using `plone.restapi`
- Make `Meeting` and `MeetingItem` implements `IATMeetingContent(IMeetingContent)` instead `IMeetingContent` to be able to define an adapter
  for `AT` contents only
- Optimized item duplication process, remove images, advices and relevant annexes (that are not kept) using `_delObject(suppress_events=True)`
  in `zope.lifecycleevent.ObjectCopiedEvent` `onItemCopied` event handler
- In `MeetingConfig.getMeetingsAcceptingItems`, extracted computation of catalog query into `MeetingConfig._getMeetingsAcceptingItemsQuery`
- An item may be taken over by members of the `proposingGroup` when it is decided
- Include `permissions.zcml` of package `plone.app.controlpanel` before loading `plone.restapi`

#### Products.MeetingCommunes (4.1.12 → 4.1.14)

#### Version 4.1.14 (2020-06-24)

- Added `import_organizations_from_csv` to be able to import organizations from a CSV file.
  [gbastien]
- In `import_meetingsUsersAndRoles_from_csv` take into account `id` if given (fallback to normalized title if not)
  and manage extra columns `groupsInCharge`, `usingGroups` and `actif` (WF state).
  [gbastien]
- Added more `position_types` by default (first alderman to sixth alderman) in `examples_fr` profile.
  [gbastien]

#### Version 4.1.13 (2020-06-11)

- Added some methods to print an item number in different ways.
  [aduchene]

#### imio.actionspanel (1.48.1 → 1.49)

#### Version 1.49 (2020-06-24)

- Fixed broken functionnality, when an action url was a `javascript` action,
  it was not always taken into account because tag <a> `href` was not disabled
  using `event.preventDefault()`.
  [gbastien]

#### imio.helpers (0.29 → 0.30)

#### Version 0.30 (2020-06-24)

- In `content.uuidsToObjects`, get object with `brain._unrestrictedGetObject`
  in case parameter `unrestricted=True`.
  [gbastien]

#### collective.documentgenerator (3.16 → 3.17)

#### Version 3.17 (2020-06-24)

- In `AT` renderer and helper, use field accessor instead `get()` method
  to get the stored value.
  [gbastien]

#### collective.eeafaceted.dashboard (0.12 → 0.13.1)

#### Version 0.13.1 (2020-06-25)

- Check if received `pod_template` has a `max_objects` before restricting
  number of `brains` to `max_objects`.
  [gbastien]

#### Version 0.13 (2020-06-24)

- Limit the number of items that can be generated in a DashboardPodTemplate.
  [odelaere]

#### collective.iconifiedcategory (0.45 → 0.46)

#### Version 0.46 (2020-06-24)

- Make `plone.restapi` validation happy by defining default value for
  `IIconifiedCategorization.default_titles` that is not stored on the
  adapted context.
  [gbastien]

#### imio.pm.locales (4.1.14 → 4.1.16)

#### Version 4.1.16 (2020-06-24)

- Added translation for `directory.position_types` validator.

#### Version 4.1.15 (2020-06-11)

- Added translation for "wf_transition_triggered_by_application" msgid in imio.history domain.

#### imio.pm.ws (2.15 → 2.16)

#### Version 2.16 (2020-06-11)

- When adding `wf_transition_triggered_by_application` comment to
  `workflow_history`, do not use a `zope.i18nmessageid.message.Message` or
  it is stored this way in workflow_history, use a simple string and
  it will be translated by `imio.history`.
  [gbastien]

#### plonetheme.imioapps (2.16 → 2.17)

#### Version 2.17 (2020-06-24)

- plonemeetingskin : moved rules with logic to hide something
  back to plonemeting.css
  [gbastien]
- Make sure tooltipster tooltip arrow is displayed correctly
  (stay sticked to the tooltipster) when zooming in the internet browser.
  [gbastien]

## Release 4.1.18

**Date:** 2020-06-03

### Package Updates

#### Products.PloneMeeting (4.1.25 → 4.1.25.1)

#### Version 4.1.25.1 (2020-06-02)

- Fixed `Meeting.validate_date` that checks that another meeting does not already use date.
  Now it is possible to create 2 meetings one hour apart, more over we avoid `portal_catalog` search with
  `getDate=list of dates` that breaks `collective.solr` (`DateIndex` receiving a list of dates)

## Release 4.1.17

**Date:** 2020-05-28

### Package Updates

#### Products.PloneMeeting (4.1.24.1 → 4.1.25)

#### Version 4.1.25 (2020-05-28)

- Refactored the way a blank item is created to avoid impossibility to insert image during creation :

  - every items, blank or not are created from an item template, this avoid use of `portal_factory`;
  - a special not removale `Default item template` is added in the `MeetingConfig` and is used as basis for creating a blank item;
  - parameter `MeetingConfig.itemCreatedOnlyUsingTemplate` is removed, deactivating the `Default item template` is the equivalent;
  - Added upgrade step to 4107
- A MeetingConfig may be removed even if still containing items (recurring items, item templates), only real items are now considered
- Avoid multiple clicks when creating a new item, icon is disabled after click and when an edition is in progress
- Make sure every `MeetingItemRecurring` and `MeetingItemTemplate` `portal_types` are registered in `portal_factory`
- Ignore schemata `settings` while viewing the MeetingConfig (meetingconfig_view) to avoid displaying tab `Settings` when using `collective.solr`
- Adapted `PMConditionAwareCollectionVocabulary` regarding changes in `collective.eeafaceted.collectionwidget`
  where `_cache_invalidation_key` method now receives a new parameter `real_context`
- Configured `cron4plone` cron job executing `@@update-delay-aware-advices` hours to `01:45` so will be executed at `02:00` (check every hours)
- Fixed JS bug that could break dashboard when deleting an item,
  call to `updateNumberOfItems` should only be made when deleting an item on the meeting view
- In `Migrate_To_4105._uncatalogWrongBrains` do not break when getting `correct_rid` if it does not exist in `portal_catalog`
- Simplified types XML files when using `imio.zamqp.pm` or not, it led to wrong configuration when GS profile order was not correct.
  `imio.zamqp.pm` is now a direct dependency of `Products.PloneMeeting`
- Added `utils._base_extra_expr_ctx` to use each time we use `collective.behavior.talcondition.utils._evaluateExpression`,
  it will return base extra context for the TAL expression, including `tool`, `cfg`, `pm_utils` and `imio_history_utils`
- In testing `PMLayer`, check if user exists before creating his memberarea as this layer is used by external packages (`imio.pm.wsclient`)

#### Products.MeetingCommunes (4.1.11 → 4.1.12)

#### Version 4.1.12 (2020-05-28)

- Call migration to PloneMeeting 4107 in migration to MeetingCommunes 4.1.
  [gbastien]
- Do not use relative path to define icon path of ItemAnnexTypeDescriptor.
  [gbastien]

#### imio.actionspanel (1.47 → 1.48.1)

#### Version 1.48.1 (2020-05-26)

- Requires `imio.helpers`.
  [gbastien]

#### Version 1.48 (2020-05-26)

- In `DeleteGivenUidView.__call__`, use `imio.helpers.content.uuidsToObjects`
  with parameter `check_contained_uids=True` to get the object to delete,
  so if not found querying with `UID` index, it will use the `contained_uids`
  index if it exists in the `portal_catalog`.
  [gbastien]

#### imio.helpers (0.27 → 0.29)

#### Version 0.29 (2020-05-28)

- Added parameter `unrestricted=False` to `content.uuidsToCatalogBrains` and
  `content.uuidsToObjects`, when `True`, catalog search is done unrestricted.
  [gbastien]

#### Version 0.28 (2020-05-26)

- Added `outputMimeType` parameter to `richtextval` method
  [sgeulette]
- Added parameter `query={}` to `content.uuidsToCatalogBrains`, this let's you
  complete the catalog query in case you have `UIDs` and you want to filter
  it on additional index like `review_state`.
  [gbastien]
- Added new parameter `catalog_id='portal_catalog'` to methods
  `catalog.addOrUpdateIndexes`, `catalog.removeIndexes`,
  `catalog.removeColumns` and `catalog.reindexIndexes` so it is possible to
  proceed with another catalog than `portal_catalog`.
  [gbastien]
- Added parameter `check_contained_uids=False` to
  `content.uuidsToCatalogBrains` and `content.uuidsToObjects`,
  when set to `True`, if query on `UID` index returns nothing, it will query on
  `contained_uids` index if it exists in the `portal_catalog` that is a special
  index used to index `UIDs` of contained elements that are not indexed.
  [gbastien]
- Added `IContainerOfUnindexedElementsMarker` marker interface to mark objects
  containing unindexed objects.
  [gbastien]

#### collective.contact.plonegroup (1.27 → 1.28)

#### Version 1.28 (2020-05-26)

- In `utils.get_organizations`, do not use a `list comprehension` to turn
  result of `get_registry_organizations` into a list as it is already the case
  (was not the case a long time ago), `get_registry_organizations` returns a
  new list and values stored in the registry will not be changed anymore by
  default.
  [gbastien]

#### collective.documentgenerator (3.14 → 3.16)

#### Version 3.16 (2020-05-25)

- Fix `RuntimeError: set changed size during iteration` error in get_children_pod_template() method.
  [sdelcourt]

#### Version 3.15 (2020-05-19)

- Improve integration of stream parameter for Appy, this allow to explicitly set the value to `False`.
  The default value remain `auto`.
  [mpeeters]
- Added Transifex.net service integration to manage the translation process.
  [macagua]
- Added Spanish translation.
  [macagua]
- Updated the i18n support.
  [macagua]

#### collective.eeafaceted.collectionwidget (1.10 → 1.11)

#### Version 1.11 (2020-05-28)

- Added `real_context` parameter to `CollectionVocabulary`.
  [sgeulette]
- Use `ITALCondition` behavior to evaluate the `tal_condition` expression so
  `ITALCondition.complete_extra_expr_ctx` is taken into account.
  [gbastien]

#### collective.iconifiedcategory (0.44 → 0.45)

#### Version 0.45 (2020-05-26)

- When using `collective.solr`, brains are not `ICatalogBrain` but `PloneFlare`
  so register `IIconifiedContent` adapter for it when installed.
  [gbastien]

#### imio.pm.locales (4.1.13 → 4.1.14)

#### Version 4.1.14 (2020-05-26)

- Added translations for "Empty item is also created from an item template" functionality.
- Added translations for "Avoid multiple clicks when creating new item by disabling the icon" functionality.

#### imio.pm.ws (2.14 → 2.15)

#### Version 2.15 (2020-05-28)

- Fixed `test_ws_getItemInfosWithShowAssembly` as default value in
  `PloneMeeting` testing profile changed to test held position having a
  `&` character (non XHTML character).
  [gbastien]
- When library `chardet` is available, it wrongly detect utf-8 passed string to
  `BeautifulSoup` as being `iso-8859-1` leading to incorrect special characters.
  `chardet` is now availabe because a dependency of `collective.zamqp`.
  So pass `unicode` string to `BeautifulSoup` to avoid this.
  [gbastien]

#### imio.zamqp.pm (0.9 → 0.10)

#### Version 0.10 (2020-05-28)

- Moved all the GS types profile logic to `Products.PloneMeeting`,
  by default it will behave like if `imio.zamqp.pm` was enabled.
  [gbastien]

## Release 4.1.16

**Date:** 2020-06-04

### Package Updates

#### Products.PloneMeeting (4.1.20.2 → 4.1.24.1)

#### Version 4.1.24.1 (2020-05-14)

- Fixed `PMUsers` vocabulary to avoid duplicates when using `LDAP` where same userid  may be defined in `LDAP` and in `source_users`
- Relaunch steps `_moveMCParameterToWFA` and `_addItemNonAttendeesAttributeToMeetings` from `Migrate_To_4104` in `Migrate_To_4105`
  for some instances that had been deployed in between
- Use getIconURL to display held_position icon on meeting edit instead getIcon as the first returns full absolute_url of the icon and the last,
  only relative URL of the icon
- In `vocabularies.ContainedAnnexesVocabulary`, only get `collective.iconifiedcategory.categories` vocab when actually having annexes
- When cloning an item with `keepProposingGroup=False` and using field `MeetingItem.proposingGroupWithGroupInCharge`, make sure new set data
  for `proposingGroup/proposingGroupWithGroupInCharge/groupsInCharge` are correct and complete.
  Added parameter `include_stored=True` to `MeetingItem.listProposingGroups` and `MeetingItem.listProposingGroupsWithGroupsInCharge`
- Ignore schemata `settings` while editing an element, this avoid `MeetingItem` edit form to display a `Settings` tab when using `collective.solr`

#### Version 4.1.24 (2020-05-08)

- In `Migrate_To_4105._cleanFTWLabels`, be sure to keep old values in case still a `PersistentList` instead removing the annotation
- In `Migrate_To_4105._removeBrokenAnnexes`, manage parent's modification date to keep old value because removing an annex
  will `notifyModifiedAndReindex` it's container
- In `@@item_duplicate_form`, disable annexes if user does not have the permission to `Add annex/Add annexDecision` on future created item
- Use `OrgaPrettyLinkWithAdditionalInfosColumn` instead `PrettyLinkColumn` in dashboards displaying `persons` and `held_positions`
- Added upgrade step to 4106
- Added `Migrate_To_4106._umarkCreationFlagForEveryItems` to make sure existing items have `at_creation_flag=False`
  or it breaks `MeetingItem.setTakenOverBy/MeetingItem.setHistorizedTakenOverBy`
- Relying on `plone.formwidget.namedfile>2.0.2` required by `collective.eeafaceted.z3ctable` also fixes the problem in `PloneMeeting`,
  no need to patch url anymore in `additionalInformations` macro for `DX content`
- When creating an item from an `itemTemplate`, if a `proposingGroup` is defined on the `itemTemplate` and current user is creator for this
  `proposingGroup`, keep it on new created item
- Use `plonemeeting_activity_managers_workflow` instead `collective_contact_core_workflow` for `person` and `held_position` portal_types because
  when using `collective_contact_core_workflow`, an element in state `deactivated` is no more viewable by `Member`
- Manage missing terms for `SelectableAssemblyMembersVocabulary` and `SelectableItemInitiatorsVocabulary` as now, inactive `held_position` objects
  are no more returned by default by these vocabularies (only `active` elements are returned)
- Renamed `Products.PloneMeeting.vocabularies.selectableassociatedorganizationsvocabulary` to
  `Products.PloneMeeting.vocabularies.detailedorganizationsvocabulary` so it is easier to reuse in other contexts
- Added possibility to select organizations as item initiators (`MeetingItem.itemInitiator`) in addition to held positions
- Removed field `MeetingItem.itemIsSigned` from `meetingitem_edit`, it is managed thru the `meetingitem_view`
- Fix `Migrate_To_4105._uncatalogWrongBrains` that was breaking the `UID` index for existing objects
- Added possibility to display available items on meeting view to other users than (Meeting)Managers :

  - added parameter `MeetingConfig.displayAvailableItemsTo`, possibility to select `Application users` and every `Power obsevers` profiles;
  - renamed adaptatble method `Meeting.showRemoveSelectedItemsAction` to `Meeting.showInsertOrRemoveSelectedItemsAction`.
- Fixed links displayed in table of available items on `meeting_view` so it is correctly opened outside the available items `iframe`
- When duplicating an item, keep original `proposingGroup` if current user is creator for it, if not, creator first `proposingGroup` is used
- While updating `delay-aware advices` during night cron, add logging even if 0 items to update
  or we can not see if there was nothing to do or wrong configuration
- Refactored `MeetingItem.isPrivacyViewable` method :

  - Instead checking if current user in `proposingGroup`, `copyGroups`, ... just check if it has `View` access on item;
  - Test for `powerobservers` restriction (`MeetingConfig.restrictAccessToSecretItemsTo`) at the end to avoid an item creator
    that is also a powerobserver not having access to it's item.
- Removed `MeetingItem.sendMailIfRelevant`, use `utils.sendMailIfRelevant` instead
- Added email notification `adviceEditedOwner` that will notify the item owner when an advice is added/edited
  in addition to existing `adviceEdited` that notifies every creators of the item `proposingGroup`
- Added email notification `temPostponedNextMeeting` that will notify the item `proposingGroup` creators that item has been postponed next meeting

#### Version 4.1.23.3 (2020-04-30)

- Added ram.cache for `PMCategoryVocabulary.__call__`, the vocabulary used for annex `content_category`,
  this is useful for the `@@item_duplicate_form` that calls it many times
- Added vocabulary `Products.PloneMeeting.Users` and using it for `person.userid` field,
  this vocabulary displays the fullname and the userid

#### Version 4.1.23.2 (2020-04-29)

- In `MeetingItem.xml`, REALLY remove the action having id `duplicate_and_keep_link`...

#### Version 4.1.23.1 (2020-04-29)

- In `MeetingItem.xml`, remove the action having id `duplicate_and_keep_link`.

#### Version 4.1.23 (2020-04-29)

- Added `ZLogHandler` in `Migrator.initNewHTMLFields` and in `Migrate_To_4105._cleanFTWLabels` as these steps may take some time
- Moved `MeetingInsertingMethodsHelpMsgView` logic from `__init__` to `__call__` because errors are swallowed in `__init__`,
  moreover display `Groups in charge` next to `Group title`
- Refactored the Duplicate item functionnality :

  - Only one button `Duplicate item` left, the `Duplicate and keep link` button was removed
  - Added possibility to display the `Duplicate item` action in dashboards, added `MeetingConfig.itemActionsColumnConfig` to be able
    to show it or not in addition to actions `Delete` and `History`
  - Added parameters `keptAnnexIds` and `keptDecisionAnnexIds` to `MeetingItem.clone`
  - Added custom widget `PMCheckBoxFieldWidget` that manages `Select/unselect all`,
    rendering HTML as value label and display a clear message when field empty
  - On click, a popup is displayed with following options :

    - Keep a link to original item?
    - Select annexes to keep
    - Select decision annexes to keep
    - Annexes and decision annexes that will not be kept because using a scan_id or used annex_type is restricted to MeetingManagers
      and current user is not a MeetingManager will be displayed greyed
- In `vocabularies.BaseHeldPositionsVocabulary`, query only `held_positions` that are in `review_state` `active`,
  moreover, display the `WorkflowState` viewlet on `person view` and `held_position view`
- Fixed `showAddAnnex` and `showAddAnnexDecision` in `@@categorized-annexes`, rely on the `content_category` field vocabulary

- Fix MeetingUser migration when no gender setted

#### Version 4.1.22.1 (2020-04-24)

- Added upgrade step in upgrade to 4105 to clean `ftw.labels` annotation if it was not migrated to a `PersistendMapping`

#### Version 4.1.22 (2020-04-24)

- Optimized calls to `collective.contact.plonegroup.utils.get_organizations` and `collective.contact.plonegroup.utils.get_organization`,
  do it with `the_objects=False` anytime possible, and avoid calling it when we have the `plone_group_id` and we need the `organization UID`
- Added migration that fixes wrong paths in `portal_catalog` (paths ending with '/' because an added annex was reindexing the parent) and
  annexes without a `content_category` that occured with wrong `ConflictError` management in `collective.quickupload` (`imio.annex`)
- Fixed `MeetingItem._checkMayQuickEdit` that was giving access to `Manager` even when field condition was `False`
- Added upgrade step to 4105
- Fixed bug in batch action `StoreItemsPodTemplateAsAnnex` that kept `Temporary QR code` label in stored annex
- Make `catalog` available on `self` in `tests`
- Optimized the `Quick edit save and continue` functionnality by using `CKEditor` `AjaxSave plugin` to save data
  so the field is not reloaded and the user editing the content stays where he was

#### Version 4.1.21 (2020-04-20)

- In `ToolPloneMeeting.pasteItem`, use `adopt_roles('Manager')` instead giving local role `Manager` to the `logged in user`.
- Optimize `UpdateDelayAwareAdvicesView._computeQuery` to only consider organizations for which a delay aware advice is configured,
  this avoid very long queries that does not please `solr`
- Added faceted filter `Copy groups`:

  - Added `Products.PloneMeeting.vocabularies.copygroupsvocabulary` (faceted) and
    `Products.PloneMeeting.vocabularies.itemcopygroupsvocabulary` (MeetingItem) vocabularies
  - moved `MeetingItem.copyGroup` vocabulary from `listCopyGroups` to `Products.PloneMeeting.vocabularies.itemcopygroupsvocabulary`
  - factorized the way advices and copy groups are displayed on item view (`displayAdvisers/displayCopyGroups`)
  - adapted tests accordingly
- Display `portal_setup` profile version for PloneMeeting related packages in `@@overview-controlpanel`
- Fixed view.printAssembly method that failed when a meeting item was not in a meeting
- Fixed test_pm_ItemStrikedAssembly to test printAssembly method when a meeting item is not in a meeting

#### imio.actionspanel (1.46 → 1.47)

#### Version 1.47 (2020-04-29)

- Add Transifex.net service integration to manage the translation process.
  [macagua]
- Add Spanish translation
  [macagua]
- In `actions_panel_actions.pt`, added `<form>` around `<input>`
  to be able to use `overlays`.
  [gbastien]

#### imio.annex (2.5 → 2.7)

#### Version 2.7 (2020-05-08)

- Test if current obj provides `IAnnex` instead `IIconifiedCategorization` as
  it is no longer provided to fix a bug in `collective.iconifiedcategory`.
  [gbastien]

#### Version 2.6 (2020-04-23)

- Avoid orphan annex left without a content_category when a `ConflictError`
  occurs during file upload because upload is done by a separate `XHR request`.
  [gbastien]

#### imio.dashboard (2.6 → 2.7)

#### Version 2.7 (2020-05-08)

- Use `OrgaPrettyLinkWithAdditionalInfosColumn` instead `PrettyLinkColumn`
  in dashboards displaying persons and held_positions.
  [gbastien]

#### imio.helpers (0.26 → 0.27)

#### Version 0.27 (2020-04-20)

- Do not break in `xhtml.imagesToPath` if `<img>` use a
  wrong `resolveuid/unknown_uid`.
  [gbastien]
- Fixed tests to not use images from site `https://www.imio.be/` but
  from site `https://i.picsum.photos/`.
  [gbastien]

#### imio.migrator (1.20 → 1.23)

#### Version 1.23 (2020-05-08)

- `ZLogHandler.init` does NOT display a starting message,
  use `ZLogHandler.info` to display initial message so we know
  what we are doing.
  [gbastien]

#### Version 1.22 (2020-04-29)

- Changed `ZLogHandler` steps from 10 to 100 in `reindexIndexesFor` and
  `reindexIndexes` too avoid to fast log scrolling.
  [gbastien]

#### Version 1.21 (2020-04-23)

- Display always warnings at the end of the migration,
  display `No warnings.` if there were not.
  [gbastien]

#### collective.contact.core (1.30 → 1.32)

#### Version 1.32 (2020-05-08)

- Add Transifex.net service integration to manage the translation process.
  [macagua]
- Add Spanish translation
  [macagua]
- Removed duplicated code displaying two times the logo in organization view.
  [gbastien]

#### Version 1.31 (2020-04-07)

- Do not execute integrity check for content types that are not related to this package.
  This prevent issues with plone.app.iterate.
  [mpeeters]

#### collective.contact.plonegroup (1.26 → 1.27)

#### Version 1.27 (2020-05-08)

- Make the `OrgaPrettyLinkWithAdditionalInfosColumn` also work for `person` and `held_position`.
  [gbastien]

#### collective.documentgenerator (3.12 → 3.14)

#### Version 3.14 (2020-04-23)

- Updated get_value to test if attribute exist on object.
  [sgeulette]
- Added possibility to pass `kwargs` to `DocumentGenerationView.__call__`,
  then submethods `generate_and_download_doc` and `_generate_doc`.
  [gbastien]

#### Version 3.13 (2020-03-04)

- Improved dg-templates-listing.
  [sgeulette]

#### collective.eeafaceted.batchactions (1.3 → 1.5)

#### Version 1.5 (2020-04-23)

- Make sure elements are treated in received `uids` order. Need to rely on
  `imio.helpers` to use `content.uuidsToCatalogBrains(ordered=True)`.
  [gbastien]

#### Version 1.4 (2019-11-25)

- Added view to change labels. (button is not added)
  [sgeulette]
- Added base view to change a collective.contact.widget field.
  [sgeulette]

#### collective.eeafaceted.z3ctable (2.8 → 2.10)

#### Version 2.10 (2020-05-08)

- In `PrettyLinkWithAdditionalInfosColumn`, removed to setup around current URL
  that was necessary for displaying image and files correctly but instead,
  require `plone.formwidget.namedfile>=2.0.2` that solves the problem.
  [gbastien]

#### Version 2.9 (2020-02-25)

- Ignored EMPTY_STRING in VocabularyColumn
  [sgeulette]

#### collective.iconifiedcategory (0.41 → 0.44)

#### Version 0.44 (2020-05-08)

- Do no more make the elements using behavior marked with
  `IIconifiedCategorization` or `content_category.setter` is not working
  anymore.
  [gbastien]

#### Version 0.43 (2020-04-30)

- Adapted tests to use `file_txt` instead `file` as id for default `File`
  as `file` is also the name of the field, `portal.file` returns the `File`
  instance instead breaking because it does not have a `file` field.
  [gbastien]
- Do not break in `utils.validateFileIsPDF` while creating a new element and
  no file has been selected.
  [gbastien]

#### Version 0.42 (2020-04-29)

- Added parameter `use_category_uid_as_token=False` to
  `CategoryVocabulary.__call__` method to be able to use category/subcategory
  as term token instead the calculated content_id (default).
  [gbastien]

#### imio.pm.locales (4.1.9 → 4.1.13)

#### Version 4.1.13 (2020-05-08)

- Simplified translation "Disabled (greyed) annexes will not be kept on the new duplicated item.".
- Added translation for "Show available items to application users" functionality.
- The msgid "Preview detailled advice" was renamed to "Preview detailed advice".
- Added translations for email notifications "itemPostponedNextMeeting" and "adviceEditedOwner".

#### Version 4.1.12 (2020-04-30)

- Added back french translation for "Duplicate and keep link" in plone.po.
- Completed translation "Disabled (greyed) annexes will not be kept on the new duplicated item.".

#### Version 4.1.11 (2020-04-29)

- Simplified french translation "${number_of_annexes} annexe(s) a(ont) été stockée(s)." to "${number_of_annexes} annexes ont été stockées.".
- Added translations for the 'Duplicate item with options' functionality.

#### Version 4.1.10 (2020-04-20)

- Added translations for copyGroups faceted filter related functionality.

#### imio.zamqp.pm (0.8 → 0.9)

#### Version 0.9 (2020-04-29)

- Added test for `MeetingStoreItemsPodTemplateAsAnnexBatchActionForm` to ensure
  that `Temporary QR code` label is not used in stored annex.
  [gbastien]
- Add a `portal_message` when an annex is removed during duplication
  because it holds a `scan_id`.
  [gbastien]

## Release 4.1.15

**Date:** 2020-04-08

### Package Updates

#### Products.PloneMeeting (4.1.19.2 → 4.1.20.2)

#### Version 4.1.20.2 (2020-04-08)

- Fixed `collective.documentgenerator` helper methods `print_attendees` and `print_attendees_by_type`:

  - removed useless method `Meeting.getNonAttendees`, nonAttendee is only relevant on item, so we use `Meeting.getItemNonAttendees`;
  - added parameter `escape_for_html=True` to both methods that will escape characters not compatible with `appy.pod`.

#### Version 4.1.20.1 (2020-04-06)

- Added new optional field (decisionSuite) for item

#### Version 4.1.20 (2020-04-02)

- Add a button to save and continuing edition for rich text fields
- Fix advanced search view with collective.solr
- Small fixes in the test to improve MeetingLalouviere test run
- Fixed a misstyped condition in tests/helpers.py
- Added new type of presence for item attendee (used to ignore an attendee on some items) :

  - new meeting optional attribute `non attendee`;
  - may be used in addition to `present/absent/excused` as even an absent attendee may be set non attendee for a specific item;
  - changed parameter `patterns` on `print_in_and_out_attendees` to `custom_patterns` to be able to redefine only one single pattern
- Fixed `AskedAdvicesVocabulary` ram.cache cachekey to avoid same vocabulary used for 2 different MeetingConfigs
  (the `indexAdvisers` term on DashboardCollection was using another MeetingConfig values), moreover made it more robust in case weird context is received
- Execute the `MeetingConfig.onMeetingTransitionItemActionToExecute` TAL expressions as `Manager` in `utils.meetingExecuteActionOnLinkedItems`
  to avoid permission problems, what is defined in the configuration must be applied.
  This makes the `a power observer may only access accepted items when meeting is closed` work when current user is a `MeetingManager`,
  not a `Manager`, instead having a permission error as `MeetingItem.updateLocalRoles` is protected with the `Modify portal content` permission
- In tests WF helpers (validateItem, decideMeeting, backToState, ...) added parameter as_manager, True by default for MeetingItem related methods and
  for backToStaten and False by default for Meeting related methods.  This way we avoid as much as possible hidden permission problems
- Exclude SearchableText indexing for IAnnex objects
- Make sure CKeditor panels are dispayed correctly in popups (adding/editing advice)
- Added `MeetingConfig.removeAnnexesPreviewsOnMeetingClosure` parameter, when True, annexes previews will be deleted upon meeting closure,
  added also action on portal_plonemeeting to be able to remove every annexes previews of every items in every closed meetings
- Added `utils.fplog`, an helper to add `collective.fingerpointing`-like log messages, adapted code to use it everywhere,
  extra logging is available when :

  - an item position changed on a meeting;
  - an inherited advice is removed;
  - an item is cloned (duplicated, sent to another MeetingConfig, ...);
  - an attribute of an annex is changed (to print, confidential, ...);
  - a RichText field is quickedited;
  - annex previews are removed (when closing meeting if relevant parameter is enabled)
- Moved parameter `MeetingConfig.meetingManagerMayCorrectClosedMeeting` to a workflowAdaptation `meetingmanager_correct_closed_meeting`
- Include plugin package name and versions in `@@overview-controlpanel` in addition to versions for `PloneMeeting` and `appy`

#### imio.pm.locales (4.1.7 → 4.1.9)

#### Version 4.1.9 (2020-04-06)

- Added translations for MeetingItem.decisionSuite field.

#### Version 4.1.8 (2020-04-02)

- Added translations for improved edition functionality.
- Added translations for the 'Non attendee' functionality.
- Added translations for 'MeetingConfig.removeAnnexesPreviewsOnMeetingClosure' related functionality.
- Added translation for 'wa_meetingmanager_correct_closed_meeting' and removed translations for 'MeetingConfig.meetingManagerMayCorrectClosedMeeting'.

#### plonetheme.imioapps (2.15 → 2.16)

#### Version 2.16 (2020-04-02)

- Added configurable help icon on the site header
  [sdelcourt]
- More precise CSS selector to hide CKEditor's spellchecking ad.
  [gbastien]

#### Products.CPUtils (1.16 → 1.17)

#### Version 1.17 (2020-04-02)

- Add a function to cleanup documentviewer generated previews
  [mpeeters]
- Added redirect after order.
  [sgeulette]

## Release 4.1.14

**Date:** 2020-03-17

### Package Updates

#### Products.PloneMeeting (4.1.18 → 4.1.19.2)

#### Version 4.1.19.2 (2020-03-17)

- Fixed a bug when redefining 'group_position_type' parameter in view.printAssembly and added a test

#### Version 4.1.19.1 (2020-03-13)

- Adapted code to remove compatibility with `collective.iconifiedcategory<0.40` (before `publishable` was introduced)
- Fixed migration to 4.1 when Plone groups are stored in other Plone groups (used when `recursive_groups` plugin is enabled)

#### Version 4.1.19 (2020-03-12)

- Do no more _versionateAdvicesOnItemEdit on item when adding/removing an annex
- Adapted code to use unique IconifiedAttrChangedEvent from collective.iconifiedcategory
- Added helper method utils.normalize_id
- When storing POD template as annex, define the id to use and pass it to api.content.create or element is renamed and ObjectModifiedEvent is called 2 times
- Fixed migration to 4.1 that removed MeetingItem.proposingGroup when calling `item.setProposingGroupWithGroupInCharge(u'')`
- Optimized annex management to avoid useless process when adding/removing/changing attr value (to_print, confidential, ...) on annexes
- Fixed migration to 4.1 while migrating Plone groups that may also contain other groups in addition to users
- Fixed email notification `advice to give` when advice is `asked again` on an item in a review_state where advices are already giveable
- Added adaptable method MeetingItem._is_complete relying on MeetingItem.completeness field
- Defined CSS rule that manage RichText fields paragraph line height everywhere it is displayed (dashboard, view, CKeditor)
- In `utils.cropHTML`, avoid visual encoding problems by making sure we have unicode before calling `BeautifulSoup`
- Optimized available items query, avoid catalog query to find past meetings
- Added field person.firstname_abbreviated useable in documentgenerator helper print_attendees_by_type method
- Added parameter annexFile=None to PloneMeetingTestCase.addAnnex, to be able to use another file than FILE.txt (like a pdf, a corrupted pdf, ...)
- Give `View` access to `portal_plonemeeting` to role `Member` so application do not fail to render when logged in user is not member of any group
- Avoid item full reindex when advice is added/modified/removed, only reindex relevant indexes (added adaptable method `MeetingItem.getAdviceRelatedIndexes` to manage custom indexes to reindex)
- When advice is added/modified/removed, clean the `Products.PloneMeeting.MeetingItem.modified` cachekey volatile to clear cache for portlet_todo
- Adapted the way late items work: now an item is late for the selected preferred meeting and for every following meetings.  This way an item that was late for a meeting may also
  be presented as late item for next meeting instead only being presentable to next non frozen meeting
- Moved `MeetingItemWorkflowConditions._groupIsNotEmpty` to `ToolPloneMeeting.group_is_not_empty` so it is easier to use everywhere
- Added new field `MeetingItem.meetingManagersNotes` only viewable/editable by MeetingManagers
- Changed the default condition in which an item may be signed (`MeetingItem.isSigned`), this is now possible as soon as an item is `validated`
- Added faceted filter `Item is signed?`
- Adapted code as vocabulary `collective.contact.plonegroup.sorted_selected_organization_services` was renamed to
  `collective.contact.plonegroup.browser.settings.SortedSelectedOrganizationsElephantVocabulary`

#### imio.annex (2.4 → 2.5)

#### Version 2.5 (2020-03-12)

- Override `collective.quickupload` `QuickUploadCapableFileFactory` to avoid
  calling object added/created/modified events more than one time.
  [gbastien]
- While adding an annex, call `validateFileIsPDF` to manage the `pdf_only`
  parameter as `invariants` are not called by default.
  [gbastien]

#### imio.helpers (0.25 → 0.26)

#### Version 0.26 (2020-02-25)

- Added set_to_annotation method.
  [sgeulette]
- Always return something in annotations functions.
  [sgeulette]

#### imio.migrator (1.19 → 1.20)

#### Version 1.20 (2020-03-12)

- Added `migrator.reindexIndexes` method that mimics the Catalog method
  but let's filter `on meta_type/portal_type` and chose to `update_matadata`.
  [gbastien]

#### collective.contact.plonegroup (1.25 → 1.26)

#### Version 1.26 (2020-03-12)

- As vocabulary `ram.cache` cachekey are generated based on
  module/class names, renamed vocabularies
  `collective.contact.plonegroup.selected_organization_services` to
  `collective.contact.plonegroup.browser.settings.SelectedOrganizationsElephantVocabulary`
  and `collective.contact.plonegroup.sorted_selected_organization_services` to
  `collective.contact.plonegroup.browser.settings.SortedSelectedOrganizationsElephantVocabulary`.
  Added tests showing that cache is correctly invalidated when selected organizations changed.
  [gbastien]

#### collective.iconifiedcategory (0.38 → 0.41)

#### Version 0.41 (2020-03-12)

- Factorized events triggered when a categorized element attribute is changed
  (`to_print`, `confidential`, ...).  Now a single `IIconifiedAttrChangedEvent`
  event is triggered.  Moreover it is optimized to avoid too much process.
  [gbastien]
- Removed specific call to `IconifiedAttrChangedEvent('confidential')`
  when creating a new categorized element.
  [gbastien]
- Added `ICategorize.only_pdf` parameter making it possible to define if the
  categorized element is a file, that it can only be PDF.  Added also invariant
  on `IIconifiedCategorization` checking if file is a PDF when categorized
  element has a file field and used content_category has `only_pdf=True`.
  [gbastien]

#### Version 0.40 (2020-02-18)

- Make appearance of column in `CategorizedTabView` coherent with appearance of
  detail icon in `@@categorized-childs-infos` view,
  rely in both case on `CategorizedChildInfosView.show`
  [gbastien]

#### Version 0.39 (2019-11-26)

- Added management of `publishable` attribute like it is the case for `to_print`
  or `confidential` attributes.  Factorized when possible.
  [gbastien]

#### imio.pm.locales (4.1.6 → 4.1.7)

#### Version 4.1.7 (2020-03-12)

- Added translation for person.firstname_abbreviated field.
- Added translations for MeetingItem.meetingManagersNotes field.
- Added translation for "Item is signed?" faceted filter.

#### imio.pm.ws (2.13 → 2.14)

#### Version 2.14 (2020-03-17)

- Added method `getSingleItemInfos` that return a single item informations,
  not a list of `ItemInfo` instances.
  Result and paramaters are exactly same as `getItemInfos`.
  [gbastien]
- Make most most of data returned by `getItemInfos` nillable.
  [gbastien]
- Added parameter `showEmptyValues=1` by default to `getItemInfos`,
  making it possible to remove empty values from returned result.
  [gbastien]

#### imio.zamqp.core (0.4 → 0.5)

#### Version 0.5 (2019-09-24)

- Skip empty scan_id in highest_scan_id method.
  [sgeulette]

#### imio.zamqp.pm (0.7 → 0.8)

#### Version 0.8 (2020-03-12)

- When cloning an item, make sure annexes having a `scan_id` are not kept.
  [gbastien]
- Added test for `get_scan_id` that appends a value `Temporary` if generated
  when pod template still not stored as annex.
  [gbastien]
- Fixed tests after changes in `collective.iconifiedcategory`, do not create an
  annex at the portal root, it is an impossible usecase but create annex in an
  item stored in a PloneMeeting folder.
  [gbastien]

#### plonetheme.imioapps (2.14 → 2.15)

#### Version 2.15 (2020-03-12)

- Avoid too much padding top and left in CKeditor edit zone.
  [gbastien]
- Added a new CSS rule to hide CKEditor's spellchecking ad [aduchene]

## Release 4.1.13

**Date:** 2020-02-21

### Package Updates

#### Products.PloneMeeting (4.1.15 → 4.1.18)

#### Version 4.1.18 (2020-02-21)

- Use another msgid for WF history comments when item is created from an item template, this way old comments still works and new comments includes item template path and title

#### Version 4.1.17 (2020-02-21)

- In live search, colorize results depending on element's review_state
- In overrided "collective.iconifiedcategory.categories", include the currently stored annex content_category no matter
  it uses only_for_meeting_managers and current user is not a MeetingManager
- Added method ItemDocumentGenerationHelperView.print_public_deliberation_decided to already existing print_deliberation and print_public_deliberation,
  this will be used to render the body of an item when it is decided
- Avoid screen size changes when editing an element with RichText fields as CKeditor takes some seconds to load, fix field height
- While creating an item from an item template, store in the WF history comments from which template the item was created

#### Version 4.1.16 (2020-02-18)

- In events.onConfigOrPloneElementModified do not call _notifyContainerModified if event element is a PloneMeeting folder, a user personal folder that contains items and meetings
- Adapted MeetingItem._update_after_edit to be able to pass only some indexes to reindex, adapted async methods (change itemlisttype, itemcompleteness, ...) accordingly.
  By default, MeetingItem._update_after_edit will do a full reindex but if some specific indexes are given, only these indexes are reindexed
- Avoid useless full reindex when RichText field is edited using quick edit and when annex is added/edited/removed
- While using ToolPloneMeeting.get_orgs_for_user, use the_objects=False as much as possible as this method is cached, returned objects could behave weirdly
- Avoid an error with zope users during install when `collective.indexing` is used
- Changed the user recovery code so that it works with an "ldap" configuration. This change allows the use of notifications with an "ldap" configuration
- Fix MeetingItem.getItemSignatories so it returns an empty dict when there is no signatories
- Fixed item view template when using field `proposingGroupWithGroupInCharge`, it may be empty when used on an item template
- In `BaseDGHV.get_scan_id`, append a special value 'Temporary' to generated QR code when is it generated and still not stored as annex as it is subject to change at next generation
- Fixed bug with itemAssembly and itemSignatures edition where an item with redefined itemAssembly/itemSignatures in a non closed meeting was editable by anybody
- Fixed bug with item confidential annex shown to groupsInCharge that were actually not shown because of a typo in adapters._reader_groups (groupincharge was renamed to groupsincharge),
  the same typo was left in the tests so it was passing...  Test was adapted to double check that values stored in MeetingConfig are existing in field vocabulary
- Added possibility to configure attributes of annexes (confidentiality, to_be_printed, ...) that will only be displayed and/or editable to MeetingManagers
- Added new methods for formatting signatures, BaseDGHV.print_signatories_by_position and BaseDGHV.print_signatures_by_position.
- Adapted BaseDGHV.printAssembly to be compatible with attendees and tested it
- Override ploneview.Plone.showEditableBorder to hide the green bar for folders stored in contacts directory
- By default, hide the `sharing` tab everywhere
- Added `items-to-advice-without-hidden-during-redaction` CompoundCriterion adapter to be able to query items to advice but not consider advice hidden during redaction.
  This is useful when advice have a workflow with several states where advice is hidden during redaction by default.  In this case the search only returns advice addable on item
- Optimized the email notification `You have been set in copy of an item` to not send several emails to the same e-mail address in case several groups are in copy and a user is in
  these groups or when `group email addresses` are used
- Added optional field `Meeting.convocationDate`

#### imio.actionspanel (1.44 → 1.46)

#### Version 1.46 (2020-02-18)

- Added renderFolderContents section, rendered following flag and/or interface.
  [sgeulette]
- In `views.AsyncActionsPanelView.__call__`, remove random value `'_' (ajax_load)`
  from `**kwargs` before calling the `@@actions_panel` or `ram_cached`
  `@@actions_panel.__call__` never work as kwargs are always different.
  [gbastien]

#### Version 1.45 (2019-11-25)

- Changed sections order.
  [sgeulette]

#### imio.migrator (1.17 → 1.19)

#### Version 1.19 (2020-02-18)

- Added logging in `Migrator.reindexIndexesFor`.
  [gbastien]

#### Version 1.18 (2019-11-25)

- Added run_dependencies parameter in runProfileSteps method.
  [sgeulette]

#### imio.pm.locales (4.1.4 → 4.1.6)

#### Version 4.1.6 (2020-02-21)

- Adapted translation of history message when item was created from item template that includes now the original item template path and title.

#### Version 4.1.5 (2020-02-18)

- Added translation for 'Temporary QR code!'.
- Added translations for MeetingConfig.annexRestrictShownAndEditableAttributes related functionality.
- Added translations for Meeting.convocationDate.

#### imio.pm.ws (2.12 → 2.13)

#### Version 2.13 (2020-02-18)

- Manage field `toDiscuss` while creating new item.
  [gbastien]
- Changed the way `wfTransitions` are managed in `createItem`: if a transition
  is not available, it is ignored and next transition is tried, this way it is
  easier to manage cases where item validation WF is different for proposing
  groups.
  [gbastien]

## Release 4.1.12

**Date:** 2020-02-06

### Package Updates

#### collective.contact.core (1.27 → 1.30)

#### Version 1.30 (2020-02-06)

- Avoid an error when we try to remove a working copy from plone.app.iterate
  [mpeeters]
- Display `description` on the organization view. Field `description` may be
  filled but was not displayed.
  [gbastien]

#### Version 1.29 (2019-11-25)

- Removed overlay on heldposition actions in person view.
  [sgeulette]
- Added option to display belowcontenttitle viewlet on contact views.
  [sgeulette]

#### Version 1.28 (2019-11-04)

- Ensure than export is unicode encoding.
  [boulch]

#### collective.contact.plonegroup (1.23 → 1.25)

#### Version 1.25 (2020-02-06)

- Use `collective.contact.plonegroup.sorted_selected_organization_services`
  for `settings.IFunctionSchema.fct_orgs`
  (field for restricting a suffix to some organizations).
  [gbastien]
- In `validateSettings` invariant check if Plone group is empty using
  `getGroupMembers` that ignores `<not found>` users instead `getMemberIds`.
  [gbastien]

#### Version 1.24 (2019-11-25)

- Added group_as_str param in organizations_with_suffixes function.
  [sgeulette]

#### collective.documentgenerator (3.10 → 3.12)

#### Version 3.12 (2020-02-06)

- Added parameter `bypass_check_permission=False` to method
  `DocumentGenerationHelperView.display`, when True it bypasses read permission
  check, this is useful when context is an object that was get unrestrictively.
  [gbastien]

#### Version 3.11 (2019-12-03)

- Casted dynamically variable.
  [sgeulette]
- Added Plone 5.2 support
  [odelaere]
- Fixed RichTextATFieldRenderer default render of empty value.
  [sdelcourt]

#### collective.eeafaceted.z3ctable (2.7 → 2.8)

#### Version 2.8 (2020-02-06)

- Managed correctly a field not yet set.
  [sgeulette]
- In the `PrettyLinkWithAdditionalInfosColumn`, manage `description` manually
  as it is not present in the `@@view` widgets.
  Display it as any other fields if not empty.
  [gbastien]
- Added IconsColumn
  [sgeulette]

#### plonetheme.imioapps (2.13 → 2.14)

#### Version 2.14 (2020-02-06)

- plonemeetingskin : added icon for 'wait advices' WF action panel button.
  [gbastien]

## Release 4.1.11

**Date:** 2020-01-10

### Package Updates

#### Products.PloneMeeting (4.1.14 → 4.1.15)

#### Version 4.1.15 (2020-01-10)

- Only show the 'Add element' actions menu when Manager is on a Folder or on a MessagesConfig element, this way we avoid users changing review_state, layout our deleting the element...
- When using the tooltipster to change the MeetingItem.listType value, display the current listType value so user know what it is before changing to another value,
  especially useful on the meeting_view where current listType value is not displayed
- Make 'pm_utils' and 'imio_history_utils' available in every TAL expressions evaluated using collective.behavior.talcondition.utils._evaluateExpression, this way it is also possible
  when evaluating the TAL expression of MeetingConfig.onTransitionFieldTransforms to access the item's history and to include in a field comment added for last WF transition for example
- Display an error portal_message while creating a meeting and some recurring items could not be inserted
- Added methods ItemDocumentGenerationHelperView.print_deliberation and ItemDocumentGenerationHelperView.print_public_deliberation, this will be used to render the body of an item.
  Added method ItemDocumentGenerationHelperView.output_for_restapi that is used by plonemeeting.restapi for the @deliberation MeetingItem endpoint
- In MeetingItem._findOrderFor, in 'on_categories', do not break if an item does not have a category,
  this can be the case when categories were just enabled and a meeting already contains items without a category
- Adapted AskedAdvicesVocabulary to only keep advices that are in MeetingConfig.selectableAdvisers.
  This vocabulary is used in the faceted filter "Advices" and for field MeetingConfig.advicesKeptOnSentToOtherMC
- Added MeetingItem.validate_groupsInCharge, when enabled in MeetingConfig.usedItemAttributes, field MeetingItem.groupsInCharge is required
- In main migration to v4.1, do not refresh other catalogs that portal_catalog (bypass reference_catalog and uid_catalog)
- Removed ToolPloneMeeting.modelAdaptations and relative functionnality (bilingual, getName, ...)
- Make RichText fields of Meeting searchable, index also meeting annexes title in SearchableText index
- Added upgrade step to 4104
- Removed DashboardCollection 'searchalldecisions' and replaced it by 'searchallmeetings', this way every meetings are displayed and user may search accross all meetings
  or filter on review_state if he wants only decided meetings
- Added helper method Migrator.updateCollectionColumns to be able to update every columns for every DashboardCollections of every MeetingConfigs
- Added possibility to define groups in charge for a given MeetingCategory, the same way it is done for organization.groups_in_charge.
  New parameters MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup and MeetingConfig.includeGroupsInChargeDefinedOnCategory will make it possible to take groups in charge
  defined on the proposingGroup or on the category into account while giving access to the item or to the confidential annexes

#### appy (0.9.15 → 0.9.16)

*No changelog entries found.*

#### imio.prettylink (1.15 → 1.16)

#### Version 1.16 (2020-01-10)

- While generating not viewable URL, avoid double blank before tag title.
  [gbastien]
- Adapted `PrettyLinkAdapter.CSSClasses` to manage `<a>` tag CSS classes and
  `<span>` tag CSS classes. `additionalCSSClasses` are set on the `<a>` tag.
  [gbastien]

#### imio.pm.locales (4.1.3 → 4.1.4)

#### Version 4.1.4 (2020-01-10)

- Added translation for MeetingItem.validate_groupsInCharge error message.
- Adapted translation of 'searchallmeetings' and added translation for 'searchnotdecidedmeetings'.
- Simplified french translation for MeetingItem.manuallyLinkedItems description.
- Added translations for MeetingConfig.includeGroupsInChargeDefinedOnProposingGroup and MeetingConfig.includeGroupsInChargeDefinedOnCategory.

#### plonetheme.imioapps (2.12 → 2.13)

#### Version 2.13 (2020-01-10)

- As state color is defined on `<span>` with `imio.prettylink`,
  define `linkColor` on hover.
  [gbastien]

## Release 4.1.10

**Date:** 2019-11-27

### Package Updates

#### Products.PloneMeeting (4.1.13 → 4.1.14)

#### Version 4.1.14 (2019-11-27)

- Finally fixes advice inheritance when original advice is not delay aware and the MeetingConfig holding inherited advice has a delay aware custom adviser
- Do not make IMeeting inherits from IFacetedNavigable or it does not apply the faceted configuration when a new meeting is created because it already implements IFacetedNavigable...
  Override the IDashboardGenerablePODTemplates from collective.eeafaceted.dashboard to manage dashboard related POD templates

#### collective.eeafaceted.dashboard (0.11 → 0.12)

#### Version 0.12 (2019-11-27)

- Implement our own `IDashboardGenerablePODTemplates` adapter like it is the
  case for `collective.documentgenerator` `IGenerablePODTemplates` adapter to
  be used in the `dashboard-document-generation-link` viewlet so it is
  registered for `IFacetedNavigation` and easier to override when necessary.
  [gbastien]

## Release 4.1.9

**Date:** 2019-11-26

### Package Updates

#### Products.PloneMeeting (4.1.11 → 4.1.13)

#### Version 4.1.13 (2019-11-26)

- Fix rendering of POD templates on Meeting, was crashing because using DashboardPODTemplates, now use ConfigurablePODTemplates
- Adapted CSS and code regarding changes in imio.prettylink (state related CSS class is moved from <a> tag to inner <span>)

#### Version 4.1.12 (2019-11-26)

- Adapted code to redefine the 'IGenerablePODTemplates' adapter for context and dashboard now that 'get_all_pod_templates' and 'get_generable_templates'
  were moved from 'DocumentGeneratorLinksViewlet' to 'GenerablePODTemplatesAdapter' in 'collective.documentgenerator'
- Fixed bug when an inherited advice is unselected from original item holding the asked advice, update back predecessors so advice is no more inherited
- Fixed bug when an inherited advice is given by a power adviser on original item then item is sent to another MeetingConfig in which a delay aware advice
  is automatically asked on resulting item, the automatically asked advice must not be taken into account in place of inherited advice

#### imio.helpers (0.23 → 0.25)

#### Version 0.25 (2019-11-26)

- Added logging in `xhtml.storeImagesLocally` if unable to
  traverse to `img_path`.
  [gbastien]
- Fixed bug in `xhtml.storeImagesLocally` where an image stored in another
  Plone element having `absolute_url` starting with current element
  `absolute_url` was not stored locally.
  [gbastien]

#### Version 0.24 (2019-11-25)

- Removed wrong overrides of `collective.iconifiedcategory` translation file.
  [gbastien]
- Added optionally behavior prefix in get_schema_fields.
  [sgeulette]
- Fixed bug in `xhtml.storeImagesLocally._handle_internal_image` to be sure
  that traversed path to image does not starts with a `/` or it fails with
  a `KeyError`.  This is the case when the `Plone Site` is using a domain name.
  Make sure also traversed `img_path` element is actually an `Image`.
  [gbastien]

#### imio.prettylink (1.14 → 1.15)

#### Version 1.15 (2019-11-26)

- Removed `unittest2`.
  [gbastien]
- Moved the state related CSS class from the `<a>/<div>` tag to the `<span>`
  inner tag, this way it is easier to define CSS compatible for
  `imio.prettylink` and `imio.history`.
  [gbastien]

#### collective.documentgenerator (3.9 → 3.10)

#### Version 3.10 (2019-11-26)

- Fix test `test_get_file_is_unrestricted` by removing permission `View`
  to every roles.
  [gbastien]
- Moved the `get_all_pod_templates/get_generable_templates` logic outside the
  `DocumentGeneratorLinksViewlet` so it is easier to override.
  It is now an `IGenerablePODTemplates` adapter.
  [gbastien]

#### collective.eeafaceted.dashboard (0.10 → 0.11)

#### Version 0.11 (2019-11-26)

- Adapted override of `collective.documentgenerator` method
  `get_all_pod_templates` now that it is handled by an `IGenerablePODTemplates`
  adapter instead the `DocumentGeneratorLinksViewlet`.
  [gbastien]

## Release 4.1.8

**Date:** 2019-11-19

### Package Updates

#### Products.PloneMeeting (4.1.9 → 4.1.11)

#### Version 4.1.11 (2019-11-19)

- Relaunch upgrade step _adaptHolidaysWarningMessage while moving to version 4103

#### Version 4.1.10 (2019-11-19)

- When an annex has been modified, avoid to reindex the entire parent, only reindex relevant indexes : modified related indexes and SearchableText as annex title is indexed into it
- Integrated new column "publishable" from collective.iconifiedcategory, this is done conditionnaly if relevant version of collective.iconifiedcategory is used
- Fixed bug where 'Manager' role was removed from 'Administrators' group when saving the results in the @@usergroup-groupprefs,
  this was due to 'Manager' role not listed in the form and so removed on save.  Now every golbal roles used by the application
  are displayed, namely 'MeetingObserverGlobal', 'Manager' and 'Member' roles.  'Site Administrator' role is not displayed for now
- No more give the 'Member' role to 'AuthenticatedUsers' auto_group, this was used with old LDAP plugin that did not give 'Member' role by default.
  Now every users will get 'Member' role and every groups, including 'AuehtenticatedUsers' will not get the 'Member' role anymore
- Fixed CSS applied on selected meeting in the meeting selection box so selected value is correctly colored
- Fixed bug where it was not possible to remove a meeting containing an item having an image used in a RichText field.
  This was due to fact that when a Plone content is removed, it's container is notifyModified, this is no more done if container is an IMeetingContent
- Fixed bug with 'waiting_advices' workflow adaptation that failed to be activated if a state defined in WAITING_ADVICES_FROM_STATES did not exist

#### imio.pm.locales (4.1.1 → 4.1.3)

#### Version 4.1.3 (2019-11-19)

- Fixed typo in 'manually_linked_items_descr' french translation.

#### Version 4.1.2 (2019-11-04)

- Added translation for portal_message warning when a ftw.labels label can not be removed because used by an item.
- Adapted translation of 'Holidays warning' collective.messagesviewlet message to be less panicking.

## Release 4.1.7

**Date:** 2019-11-04

### Package Updates

#### Products.PloneMeeting (4.1.8 → 4.1.9)

#### Version 4.1.9 (2019-11-04)

- Add a validation step "Are you sure?" before launching items and meetings local roles update from the action button on portal_plonemeeting
- Fixed ftw.labels :
  - Jar storage that was a dict instead a PersistentMapping and that was making changes done to it not persisted;
  - Go back to the 'data' tab on the MeetingConfig while removing a label from the labels portlet;
  - Invalidate the ftw.labels faceted vocabulary when a label is added/updated/removed.
- While storing a POD template as annex, make sure values for form.store_as_annex and form.target are correctly set back to defaults because
  in case a user use the back button, this could lead to Unauthorized while generating a POD template that can not be stored just after having stored a POD template
- Optimize MeetingItem.updateLocalRoles to take into account cases when several items are updated :
  - Do not compute auto copy groups if there were no expression found on previous updated item of same portal_type
  - Do not update annexes accesses if annex was not confidential and still not confidential
  - Added caching to collective.contact.plonegroup.get_organization for the time of a REQUEST to avoid doing too much catalog queries
  - Added avoid_reindex parameter to updateLocalRoles method, in this case, if __ac_loca_roles__ did not change, reindexObjectSecurity is bypassed
- Use declareProtected(ModifyPortalContent) for methods on MeetingItem 'setCategory', 'setClassifier', 'setProposingGroup' and 'setProposingGroupWithGroupInCharge'
- Fixed bug when an item is sent to another MeetingConfig and fails to be presented in a meeting because none is available, it crashed to render the portal_message
  if the destination MeetingConfig title contained special characters
- Changed text of collective.messagesviewlet 'Holidays warning' message to use a less panicking content
- Added upgrade step to fix wrong ToolPloneMeeting.holidays value '2017/2/25'

#### collective.contact.core (1.26 → 1.27)

#### Version 1.27 (2019-09-20)

- Added contact_source metadata to be used in contact widget.
  [sgeulette]
- If person details privacy is True, contact details on person don't search related items.
  [sgeulette]

#### collective.contact.plonegroup (1.22 → 1.23)

#### Version 1.23 (2019-11-04)

- Added parameter `caching=True` to `utils.get_organization`, this will store
  the organization object in the REQUEST and avoid too much catalog queries.
  [gbastien]

## Release 4.1.6

**Date:** 2019-10-14

### Package Updates

#### Products.PloneMeeting (4.1.7 → 4.1.8)

#### Version 4.1.8 (2019-10-14)

- Added possibility to bypass catalog/workflows refresh in migration step to 4101 if coming from migration step to 4.1 as this was already done
- Adapted AdvicesIconsInfos.mayRemoveInheritedAdvice that is also used by the '@@advice-remove-inheritance' view
  so a MeetingManager may remove an inherited advice as long as item is not decided
- Display workflowstate viewlet the new way as it was moved to plonetheme.imioapps and CSS were changed
- Show clearly empty lines at end of Meeting.signatures field, this way editors may see immediatelly if a line is missing
- Fixed vocabulary keys used for field MeetingConfig.mailMeetingEvents (listMeetingEvents) that was breaking the mail notifications upon meeting state change
- Fixed migration step Migrate_To_4101._correctAccessToPODTemplates to also update StyleTemplate objects
- Fixed itemsignatures management to keep empty lines at the end of the value because it was stripped by the form

#### imio.migrator (1.16 → 1.17)

#### Version 1.17 (2019-10-14)

- Add some more logging for actions `Clear and rebuild` or `Refresh` catalog.
  [gbastien]
- Added parameter `catalogsToUpdate` to `refreshDatabase` so we can define what
  catalog will be refreshed because by default, every catalogs are refreshed
  and it is rarely necessary.
  [gbastien]

#### collective.documentgenerator (3.8 → 3.9)

#### Version 3.9 (2019-10-14)

- context_var returns default when value is None.
  [sgeulette]
- While reusing another POD template odt_file, make sure get_file will have
  access to the POD template holding the odt_file by getting it unrestricted.
  [gbastien]
- Fixed test `TestDexterityHelperViewMethods.test_display_date_method` as
  translation format changed starting with `Plone 5.1.x`.
  [gbastien]

#### collective.messagesviewlet (0.20 → 0.21)

#### Version 0.21 (2019-10-14)

- Bypass allowed content types contraint when (post)install messagesConfig container
  [boulch]

#### imio.pm.locales (4.1 → 4.1.1)

#### Version 4.1.1 (2019-10-14)

- Adapted translation of field IPMHeldPosition.secondary_position_type so it is clear that it is not an additional held_position.

#### imio.pm.ws (2.11 → 2.12)

#### Version 2.12 (2019-10-14)

- Do not fail in 'getItemInfos' when returning POD templates if a POD template
  is using the odt_file of another POD template.
  [gbastien]

#### plonetheme.imioapps (2.11 → 2.12)

#### Version 2.12 (2019-10-14)

- Use common CSS for workflowstate viewlet.
  [gbastien]

## Release 4.1.5

**Date:** 2019-10-04

### Package Updates

#### Products.PloneMeeting (4.1 → 4.1.7)

#### Version 4.1.7 (2019-10-04)

- Fixed bug where an error was raised when asking a delay aware advice on an item for which an non delay aware inherited advice was already existing.
  Adapted MeetingItem.validate_optionalAdvisers to not let select an adviser if it is already inherited on current item
- Added migration step to make sure POD templates access is fixed
- Corrected template 'export-organizations.ods' as field PMOrganization.selectable_for_plonegroup was removed
- In migration to v4.1, migrate also expressions using 'here' ('here.portal_plonemeeting', ...)

#### Version 4.1.6.1 (2019-10-01)

- In Migrate_To_4_1._updateUsedAttributes while already migrated

#### Version 4.1.6 (2019-10-01)

- Moved the logic of added a line to the workflow_history while creating an new item to utils.add_wf_history_action so it can be used by other packages (imio.p.ws)
- Removed @ram.cache for MeetingConfig.listStates method, this was sometimes leading to breaking the workflowAdaptations application and validation
- Fixed migration to 4101, in _removeTagsParameterInCallToJSCallViewAndReloadInCloneToOtherMCActions, do not call MeetingConfig._updatePortalTypes because it does not apply
  workflowAdaptations, call MeetingConfig.registerPortalTypes
- print_meeting_date : Backward compatibility with old PODTemplates

#### Version 4.1.5 (2019-09-30)

- Fixed migration of contacts/orgs-searches 'c5.default' faceted criterion as we store a string instead a list, we can not use the 'edit'
  method that validates the format of the given value

#### Version 4.1.4 (2019-09-30)

- Added 'MeetingItem.groupsInCharge' to 'MeetingConfig.ItemFieldsToKeepConfigSortingFor' so it is possible to display it alphabetically
  or keep order defined in 'MeetingConfig.orderedGroupsInCharge'
- Adapted 'MeetingItem.getAdviceObj' to not use the MeetingItem.adviceIndex 'advice_id' to get the given advice.
  Indeed, when this method is called during 'MeetingItem.adviceIndex' computation, the 'advice_id' could not be there even if advice obj exists
- Fixed access to item view to users not able to view the linked meeting.  Indeed in this case it raised Unauthorized because call to Meeting.getAssembly (now declared Public)
- Adapted the item edit form to display fields 'proposingGroup', 'proposingGroupWithGroupInCharge', 'groupsInCharge', 'classifier' and 'category' one below the others
  and no more one next the the other to avoid hidding fields when one field is too large
- Adapted print_meeting_date and print_preferred_meeting_date so they can now be used in restricted or unrestricted mode
- Adapted migration to 4101 to make sure that value stored in 'c5' widget of contacts/orgs-searches dashboard is not a list

#### Version 4.1.3 (2019-09-23)

- Fixed bug "AttributeError: 'NoneType' object has no attribute 'lower'" in BaseDGHV.printAdvicesInfos when advice comment is None
- Added parameter ordered=True to 'MeetingItem.getAdvicesByType', this will order elements by adviser group title (key 'name' in indexAdvisers) under an advice_type
- Fixed migration, do not fail to migrate 'MeetingItem.copyGroups' in case a copy group does not exist anymore, was possible in old versions
- Added field held_position.secondary_position_type working exactly the same way as held_position.position_type to be able to define a secondary_position_type useable when necessary.
  Adapted also held_position.get_prefix_for_gender_and_number method to be able to pass position_type_attr='secondary_position_type'
- Added 'MeetingItem.associatedGroups' to 'MeetingConfig.ItemFieldsToKeepConfigSortingFor' so it is possible to display it alphabetically
  or keep order defined in 'MeetingConfig.orderedAssociatedOrganizations'
- Added back informations in meetingitem_view about items defined in tool (templateUsingGroups/meetingTransitionInsertingMe), was removed wrongly when removing the 'back' link
- Added inserting method 'on_item_title', this will insert items following title alphabetical order
- Added inserting method 'on_item_decision_first_words', this will insert items following decision field content alphabetical order
- Added inserting method 'on_item_creator', this will insert items following item creator fullname alphabetical order
- Fixed Migrator.updateTALConditions to use the behavior adapter to get/set the tal_condition

#### Version 4.1.2 (2019-09-13)

- Defined 'Products.PloneMeeting.vocabularies.everyorganizationsvocabulary' only calling original 'collective.contact.plonegroup.every_organizations' vocabulary
  but adds ram.cache and render term title without "My organization"
- Use vocabulary 'Products.PloneMeeting.vocabularies.associatedgroupsvocabulary' for faceted filter 'associatedGroups' instead
  'Products.PloneMeeting.vocabularies.everyorganizationsacronymsvocabulary'

#### Version 4.1.1 (2019-09-12)

- Fixed bug on item template view when no proposingGroup defined, be defensive when getting proposingGroup
- In the "Products.PloneMeeting.vocabularies.groupsinchargevocabulary", only consider organizations selected in plonegroup
- Disable "inline_validation.js"
- Added new advice types "Cautious" and "Positive with comments", in addition to default ones "Positive, Positive with remarks, Negative and Nil"
- Added possibility to filter item dashboards for items taken over by "Nobody"
- Use natsort.humansorted instead natsort.realsorted to sort vocabularies by term title
- Changed base implementation of MeetingWorkflowConditions.mayDecide to only check if current user has "Review portal content" permission
- Make the searchlastdecisions meetings search able to display decisions in the future
- Do not display the 'review_state' columns in contacts dashboard displaying organizations, it is always 'active', we use the 'selected in plonegroup' column information instead
- Fixed migration of MeetingUsers, do not fail if a MeetingUser was deleted and initialize MeetingConfig.orderedContacts and MeetingConfig.orderedItemInitiators correctly
- Added possibility to use a DashboardPODTemplate added into the contacts directory on contacts dashboards (and to define it in an import_data as well)
- Moved organization.selectable_for_plonegroup field to the 'app_parameters' fieldset
- Handle display of tooltipster when "tap" event (when using application on a mobile device)
- Adapted actions_panel and faceted collection widget vocabulary to invalidate cache when portal_url changed, this can be the case when accessing application thru different portal_url
- Make Products.PloneMeeting.utils package available in POD templates under name 'pm_utils', it is already the case under name 'utils'
- Removed the organization.selectable_for_plonegroup attribute, organizations not selectable in plonegroup will be stored outside plonegroup organization
- Added possibility to import organization in a parent when using the organizations.csv to import contacts
- Moved the MeetingItem.optionalAdvisers vocabulary from MeetingItem.listOptionalAdvisers to vocabulary factory 'Products.PloneMeeting.vocabularies.itemoptionaladvicesvocabulary',
  this is necessary for imio.pm.ws to handle asking advices when using the createItem SOAP method
- JS method 'callViewAndReload' was moved to imio.helpers, moreover, useless parameter 'tags' was removed
- Added holidays for 2020 and added corresponding upgrade step
- Added parameter "include_person_title" to held_position.get_prefix_for_gender_and_number making it possible to generate "Madame la Directrice" sentence
- Use vocabulary 'collective.contact.plonegroup.sorted_selected_organization_services' instead 'collective.contact.plonegroup.selected_organization_services'
- Added utils.uncapitalize to lowerize first letter of a given string
- Moved MeetingConfig.onMeetingTransitionItemTransitionToTrigger to MeetingConfig.onMeetingTransitionItemActionToExecute, in addition to be able to trigger a transition on every items
  of a meeting when a transition is triggered on a meeting, it is now possible to execute a TAL expression
- 'workflowstate' viewlet was moved to plonetheme.imioapps.browser.viewlets and utils.get_state_infos was moved to imio.helpers.content, adapted code accordingly
- Added Ability to run using solr instead of catalog
- Do not restrict selection of held_position.position to organizations outside "My organization".  We may link an held_position to an organization stored in "My organization".
  This will let link a held_position to an organization having a role in the application: group in charge, adviser, ...
- Changed organization.get_certified_signatures parameter from_group_in_charge=False to group_in_charge=None, it will receive a group in charge (organization) to get certified signatures on.
  This manage the fact that several groups in charge may be selected on an organization and the selected group in charge is defined on the linked item
- Override organization.get_full_title only when value is not the indexed value. So "My organziation" is displayed in the contact widget but not in other cases

#### imio.actionspanel (1.42 → 1.44)

#### Version 1.44 (2019-09-13)

- By default, do not display the `Edit` action when calling
  `@@async_actions_panel`.
  [gbastien]

#### Version 1.43 (2019-09-12)

- Disabled first option of add content button list.
  [sgeulette]
- Added apButtonSelect class on select button
  [sgeulette]
- Do not link anymore showEdit to showIcons.
  Disabled by default showEdit in viewlet.
  Render edit as button too.
  [sgeulette]

#### imio.helpers (0.22 → 0.23)

#### Version 0.23 (2019-09-12)

- Added `content.get_vocab` helper method to easily get a `IVocabularyFactory`
  vocabulary instance or only the factory when parameter `only_factory=True`.
  [gbastien]
- Added `catalog.reindexIndexes` helper method making it possible to reindex a
  specific `portal_catalog` index with `ZLogHandler` log output.
  [gbastien]
- Added javascript function to callViewAndReload with ajax. Gotten from PloneMeeting ;-)
  [sgeulette]
- Added get_state_infos (used in PM and plonetheme.imioapps).
  [sgeulette]

#### imio.history (1.18 → 1.19)

#### Version 1.19 (2019-10-01)

- Allow access to module `utils` from restricted python (TAL expression).
  [gbastien]

#### imio.migrator (1.14 → 1.16)

#### Version 1.16 (2019-09-12)

- Added `Migrator.reindexIndexesFor(idxs=[], **query)` method to be able to
  easily reindex given `idxs` (indexes) on brains returned by
  a given catalog `query`.
  [gbastien]

#### Version 1.15 (2019-09-12)

- Highlight log message about warning messages encountered durung migration.
  [gbastien]
- Fixed `Migrator.refreshDatabase` method, wfs passed to
  `WorkflowTool._recursiveUpdateRoleMappings` need to be a dict with
  `wf id` as `key` and `wf object` as `value`, we had `wf object` for `key`
  and `value`.
  [gbastien]

#### collective.contact.plonegroup (1.19 → 1.22)

#### Version 1.22 (2019-09-26)

- When passing `kept_org_uids` to `utils.get_organizations`,
  make sure order is preserved.
  [gbastien]

#### Version 1.21 (2019-09-13)

- Added `BaseOrganizationServicesVocabulary._term_title` to ease override of
  rendered term title.
  [gbastien]

#### Version 1.20 (2019-09-12)

- Added `collective.contact.plonegroup.every_organizations` vocabulary, to do
  this needed to write `BaseOrganizationServicesVocabulary` from which
  `OwnOrganizationServicesVocabulary` and `EveryOrganizationsVocabulary`
  inherits.
  [gbastien]
- Removed sorting on term title for
  `collective.contact.plonegroup.selected_organization_services`, terms are
  displayed following selection order in plonegroup organizations like before.
  Added new vocabulary sorted on term title and available as
  `collective.contact.plonegroup.sorted_selected_organization_services`.
  [gbastien]

#### collective.eeafaceted.collectionwidget (1.9 → 1.10)

#### Version 1.10 (2019-09-12)

- Invalidate `collective.eeafaceted.collectionwidget.cachedcollectionvocabulary`
  if `portal_url` changed, this can be the case when application is accessed
  by same user from different URi.
  [gbastien]

#### collective.eeafaceted.z3ctable (2.5 → 2.7)

#### Version 2.7 (2019-09-13)

- In `columns.AbbrColumn`, make sure there is no `'` in tag title or it is not
  rendered correctly in the browser.
  [gbastien]

#### Version 2.6 (2019-09-12)

- Fixed translation of `Please select at least one element.` msgid, it was
  still using the old domain `collective.eeafaceted.batchactions` from which
  the `select_row` column was reintegrated.
  [gbastien]
- Optimized the `PrettyLinkWithAdditionalInfosColumn` speed :

  - the `view.update` is called one time and we store the view in the column
    so next rows may use it;
  - use `collective.excelexport` datagridfield exportable to render a
    `datagridfield` because widget rendering is way too slow...
  - added `collective.excelexport` as a dependency.

  [gbastien]

#### collective.excelexport (1.7 → 1.8)

#### Version 1.8 (2019-09-12)

# BREAKING CHANGES

CONFIGURATION_FIELDS constant has been removed, we now use a registry record: collective.excelexport.excluded_exportables

# CHANGES

- Explicit inclusion of plone.restapi zcml
  [thomasdesvenain]

- Exclude dexterity 'allow discussion' and 'exclude_from_nav' fields
  (previously, only archetypes fields were excluded)
  [thomasdesvenain]

- Fix error when referenced object value has no Title method.
  [thomasdesvenain]

- Fix: Don't ommit fields that are in the default fieldset if there is one
  [petchesi-iulian]

- Fix error on eea.faceted when there is a widget operator.
  [thomasdesvenain]

- Archetypes support,
  Products.ATExtensions support (RecordField, RecordsField, FormattableNamesField).
  [thomasdesvenain]

- Fix encoding issue.

#### collective.js.tooltipster (1.3 → 1.4)

#### Version 1.4 (2019-09-12)

- Set `async:true` for ajax request when no `functionReady_callback` provided.
  [gbastien]
- By default, make `click/tap/mouseenter` open a `tooltipster` and
  `click/tap/mouseleave` close it. This makes it useable on mobile devices.
  [gbastien]

#### imio.pm.locales (4.1rc4 → 4.1)

*No changelog entries found.*

#### imio.pm.ws (2.7 → 2.11)

#### Version 2.11 (2019-10-01)

- Make it easier to detect if an item was created using the createItem SOAP WS
  by adding a specific line to the item workflow_history like it is the case
  when creating an item from an item template or from a recurring item.
  [gbastien]

#### Version 2.10 (2019-09-30)

- 'getItemInfos' returns 'meeting' containing the meeting UID if any.
  [gbastien]
- 'searchItems' now accepts an additional search parameter 'linkedMeetingUID'.
  [gbastien]

#### Version 2.9 (2019-09-24)

- In 'getItemInfos' when 'showAssembly=True', changed separator between list of
  assembly members from '|' to '\n' so it is easier to parse as '|' is already
  the separator between types of attendees (attendees, absents, excused, ...).
  [gbastien]

#### Version 2.8 (2019-09-23)

- In createItem, added possibility to define associatedGroups and
  groupsInCharge as lists of organization UIDs.
  [gbastien]
- Added parameter 'wfTransitions' to createItem making it possible to trigger
  given WF transitions on the newly created item.
  [gbastien]
- In createItem, added possibility to define optionalAdvisers.
  [gbastien]
- Force catalog query in getItemInfos to use 'sort_on=created'.
  [gbastien]
- In getItemInfos, added 'showAssembly=False' parameter making it possible to
  receive the item assembly in the _item_assembly attribute when item is in a
  meeting.
  [gbastien]
- Removed manual handling of currentWSDL.txt.  Now dumpedWSDL.txt is generated
  by calling 'http://portal_url/@@ws4pm.wsdl?dump_wsdl:boolean=True'.
  [gbastien]
- Added parameter 'allowed_annexes_types' and 'include_annex_binary' to 
  getItemInfos() method.
  [sdelcourt]
- Add attribute 'id' to the AnnexInfo data type.
  [sdelcourt]

#### plonetheme.imioapps (2.10 → 2.11)

#### Version 2.11 (2019-09-12)

- Added style for apButtonSelect class of actionspanel.
  [sgeulette]
- Added CSS for datagridfield rendered in a dashboard additional infos column.
  [gbastien]
- Added workflowstate viewlet
  [sgeulette]
- Added css for apButtonAction_edit.
  [sgeulette]

## Release 4.1.4

**Date:** 2019-08-23

### Package Updates

#### Products.PloneMeeting (4.1b17 → 4.1)

*No changelog entries found.*

#### appy (0.9.14 → 0.9.15)

*No changelog entries found.*

#### imio.actionspanel (1.40 → 1.42)

#### Version 1.42 (2019-06-28)

- Store result of `ActionsPanelView.getTransitions` in `self._transitions` as
  it is called several times to make sure transitions are computed only one time.
  [gbastien]
- In `ConfirmTransitionView`, store the actionspanel view instead instanciating
  it several times as call to `actionspanel.getTransitions` is cached on the
  actionspanel view.
  [gbastien]

#### Version 1.41 (2019-06-07)

- In `load_actions_panel JS function`, do not reload in case of error or the
  page is reloaded ad vitam.  Display an error message instead.
  [gbastien]
- When using `string:` expressions, do not insert a blank space like
  `string: `` or it is kept once rendered.
  [gbastien]
- Manage `IGNORABLE_ACTIONS` the same way `ACCEPTABLE_ACTIONS` so we filter out
  first every non relevant actions then we evaluate it.
  Removed management of `IGNORABLE_CATEGORIES` and `IGNORABLE_PROVIDERS`, we
  only keep `object_buttons` and providers `portal_actions/portal_types`.
  [gbastien]

#### imio.helpers (0.18 → 0.22)

#### Version 0.22 (2019-08-23)

- Added parameter `update_metadata` to `catalog.addOrUpdateColumns`,
  if `True` (default), the new added metadata are updated on every
  catalogued objects.
  [gbastien]
- Added function to return html link for an object
  [sgeulette]

#### Version 0.21 (2019-08-13)

- Added parameter `get_again=False` to
  `cache.invalidate_cachekey_volatile_for`, when True, this will call
  `cache.get_cachekey_volatile` just after the cache is invalidated so we get
  a fresh date stored. This is useful to avoid write by async requests if it
  calls `cache.get_cachekey_volatile`.
  [gbastien]

#### Version 0.20 (2019-07-19)

- In `xhtml.storeImagesLocally`, do not break when a `resolveuid` is found but
  it does not find the image. This can be the case when copy/pasting HTML code
  from another instance or so.
  [gbastien]
- In `xhtml.removeBlanks`, check if content is empty by calling
  `xhtml.xhtmlContentIsEmpty` with parameter `tagWithAttributeIsNotEmpty=False`
  so empty tags with attributes are considered empty.
  [gbastien]

#### Version 0.19 (2019-07-05)

- Patch index method from collective.solr to fix an issue with partial reindex
  [mpeeters]
- Added css id on row field display in container.pt and content.pt.
  [sgeulette]

#### imio.migrator (1.11 → 1.14)

#### Version 1.14 (2019-07-19)

- Use same format when displaying duration of migration, duration is displayed
  in days/hours/minutes/seconds in any cases.
  [gbastien]

#### Version 1.13 (2019-06-28)

- Be more preceise regarding duration of migration
  (display in seconds and hours/minutes).
  [gbastien]

#### Version 1.12 (2019-06-14)

- Migrator class is no more an old-style class (it inherits from object now).
  [gbastien]

#### collective.contact.core (1.25 → 1.26)

#### Version 1.26 (2019-06-28)

- Set `cacheable="True"` for `style.css` in `cssregistry.xml`.
  [gbastien]
- Keep div and CSS id `viewlet-below-content-body` when rendering
  `plone.belowcontentbody` viewlets on various views.
  [gbastien]
- Extended `utils.get_gender_and_number` to manage parameters `use_by` and
  `use_to` that will add new values to returned result prepended by
  `'B'` or `'T'`.
  [gbastien]
- Added email index
  [sgeulette, daggelpop]

#### collective.contact.plonegroup (1.14 → 1.19)

#### Version 1.19 (2019-08-23)

- Optimized `OwnOrganizationServicesVocabulary.listSubOrganizations`, do the
  catalog query only if current organization contains something.
  [gbastien]

#### Version 1.18 (2019-08-02)

- In `OrgaPrettyLinkWithAdditionalInfosColumn`, set `showContentIcon` to True
  and enable `link-tooltip`.
  [gbastien]
- In `SelectedInPlonegroupColumn`, display `Not` in bold.
  [gbastien]
- Added `collective.contact.plonegroup.functions` vocabulary listing every
  functions defined in plonegroup control panel.
  [gbastien]

#### Version 1.17 (2019-07-15)

- Corrected bad full title shortening.
  [sgeulette]

#### Version 1.16 (2019-06-30)

- Fixed error in `OrgaPrettyLinkWithAdditionalInfosColumn` when displaying
  organizations out of `PLONEGROUP_ORG`.
  [gbastien]
- Fixed `utils.get_organizations` when `caching=True` to store a new list of
  organizations in the cache instead returned value or value in cache may be
  modified if we modify returned value in a sub method...
  [gbastien]
- Use `get_registry_organizations/set_registry_organizations` and
  `get_registry_functions/set_registry_functions` as much as possible.
  [gbastien]

#### Version 1.15 (2019-06-07)

- Fixed problem, linked Plone groups title were not updated when suffix title
  changed and some `fct_orgs` were defined.
  [gbastien]
- In `settings.detectContactPlonegroupChange`, set `changes = True` only when
  relevant, due to wrong indentation, it was done systematically.
  [gbastien]

#### collective.documentgenerator (3.7 → 3.8)

#### Version 3.8 (2019-08-13)

- Added custom temporary directory 'CUSTOM_TMP' environment variable
  for appy's workspace.
  [odelaere]
- Added ability to use an external server process for LibreOffice.
  [odelaere]
- Make `DocumentGeneratorLinksViewlet.get_links_info` return also the
  `pod_template object` in addition to `pod_template UID`.
  [gbastien]

#### collective.eeafaceted.collectionwidget (1.7 → 1.9)

#### Version 1.9 (2019-08-23)

- Added parameter `raise_on_error=True` to `utils._get_criterion` so it will
  return `None` in case passed context is not a faceted context instead
  raising an error.
  [gbastien]

#### Version 1.8 (2019-08-13)

- Do not store the collection object in `term.value` of vocabulary
  `CollectionVocabulary` because it can be ram cached
  (in `CachedCollectionVocabulary` for example) and ram caching methods
  returning objects is a bad idea.
  [gbastien]
- Added `caching=True` parameter to `utils.getCurrentCollection` so it is
  computed one time by request for a given `faceted_context`.
  [gbastien]

#### collective.eeafaceted.dashboard (0.8 → 0.10)

#### Version 0.10 (2019-08-13)

- Adapted code to render term as term.value does not contain the collection
  object anymore but it's path.
  [gbastien]
- Do not compute kept_criteria when widget is rendered outside dashboard as
  faceted criteria will not be displayed.
  [gbastien]
- Use `collectionwidget.utils.getCurrentCollection` to get the current
  collection to use for `DashboardFacetedTableView` columns.
  [gbastien]

#### Version 0.9 (2019-06-07)

- Added function utils.addFacetedCriteria to ease applying a faceted conf xml
  that adds extra faceted criteria to an existing dashboard.
  [gbastien]
- Improved template evaluate method to avoid getting collection and criterias
  if not necessary
  [sgeulette]
- Display dashboard-document-generation-link only on IFacetedNavigable
  [sgeulette]
- Corrected robot tests
  [sgeulette]

#### collective.eeafaceted.z3ctable (2.4 → 2.5)

#### Version 2.5 (2019-08-02)

- In `VocabularyColumn` and `AbbrColumn`, store the vocabularies instances
  under `_cached_vocab_instance` to avoid doing a lookup for each row.
  This does speed rendering a lot.
  [gbastien]

#### collective.iconifiedcategory (0.36 → 0.38)

#### Version 0.38 (2019-08-23)

- Fixed code to work with `plone.app.async` as in this case, there is no
  `REQUEST`.  To do this, needed to get the `@@images` view by instantiating the
  `ImageDataModifiedImageScaling` class, this could be a problem if it is
  overrided by a subpackage.
  [gbastien]
- Tried to fix again tooltipster popup when categorized element title is
  displayed on several lines...
  [gbastien]

#### Version 0.37 (2019-06-14)

- Avoid vertical scroll in tooltipster popup when categorized content title
  is displayed on several lines.
  [gbastien]
- Force use distribution trusty in Travis.
  [gbastien]

#### collective.messagesviewlet (0.17 → 0.20)

#### Version 0.20 (2019-08-23)

- Added parameter `caching=True` to `utils.get_messages_to_show`, if `True`,
  the method result is cached in the request for given `context`.
  [gbastien]

#### Version 0.19 (2019-07-15)

- Added PseudoMessage class that be be used in viewlet template.
  [sgeulette]

#### Version 0.18 (2019-05-27)

- Define version to `2000` in `metadata.xml` of plone4 profile or upgrade step
  to 2000 is always displayed.
  [gbastien]

#### imio.pm.locales (4.1b13 → 4.1rc4)

*No changelog entries found.*

#### plonetheme.imioapps (2.8 → 2.10)

#### Version 2.10 (2019-06-28)

- Set `collective.behavior.talcondition` input field `width` to `99%`.
  [gbastien]

#### Version 2.9 (2019-06-08)

- Set `padding-top: 0.5em;` instead `padding-top: 1em;` for
  `td.table_widget_value` so it is the same value as for
  `td.table_widget_label` and label/value are correctly aligned in views
  using it (our default dexterity view).
  [gbastien]

#### Products.CPUtils (1.14 → 1.16)

#### Version 1.16 (2019-08-23)

- Corrected list_users.
  [sgeulette]
- Improved object_link function.
  [sgeulette]

#### Version 1.15 (2019-06-08)

- The list_users method returns also global roles of groups/users.
  [odelaere]