---

database-plugin: basic

---

```yaml:dbfolder
name: new database
description: new description
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 1
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  QuickNotes:
    input: text
    accessorKey: QuickNotes
    key: QuickNotes
    id: QuickNotes
    label: QuickNotes
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  To:
    input: text
    accessorKey: To
    key: To
    id: To
    label: To
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  From:
    input: text
    accessorKey: From
    key: From
    id: From
    label: From
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Date_Sent:
    input: text
    accessorKey: Date_Sent
    key: Date_Sent
    id: Date_Sent
    label: Date Sent
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  WhichParty:
    input: select
    accessorKey: WhichParty
    key: WhichParty
    id: WhichParty
    label: WhichParty
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Party1", value: "Party1", color: "hsl(68, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  NoteIcon:
    input: select
    accessorKey: NoteIcon
    key: NoteIcon
    id: Notetype
    label: Note Icon
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Letter", value: "Letter", color: "hsl(198, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
  Status:
    input: select
    accessorKey: Status
    key: Status
    id: status
    label: status
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Delivered", value: "Delivered", color: "hsl(143, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
config:
  remove_field_when_delete_column: false
  cell_size: compact
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: z_Templates/1. DM Templates/Template - Letters.md
  pagination_size: 10
  font_size: 16
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: dd-MM-yyyy
  datetime_format: "dd-MM-yyyy HH:mm:ss"
  metadata_date_format: "dd-MM-yyyy HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: false
  conditions:
```