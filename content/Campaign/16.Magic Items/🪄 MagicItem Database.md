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
  Art:
    input: text
    key: Art
    accessorKey: Art
    label: Art
    position: 2
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
  type:
    input: select
    accessorKey: type
    key: type
    id: type
    label: type
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Rod", value: "Rod", color: "hsl(166, 95%, 90%)"}
      - { label: "Trinket", value: "Trinket", color: "hsl(169, 95%, 90%)"}
      - { label: "Ring", value: "Ring", color: "hsl(187, 95%, 90%)"}
      - { label: "Weapon", value: "Weapon", color: "hsl(284, 95%, 90%)"}
      - { label: "Shield", value: "Shield", color: "hsl(178, 95%, 90%)"}
      - { label: "Wonderous Item", value: "Wonderous Item", color: "hsl(252, 95%, 90%)"}
      - { label: "Armor", value: "Armor", color: "hsl(146, 95%, 90%)"}
      - { label: "Necklace", value: "Necklace", color: "hsl(9, 95%, 90%)"}
      - { label: "Potion", value: "Potion", color: "hsl(149, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  rarity:
    input: select
    accessorKey: rarity
    key: rarity
    id: rarity
    label: rarity
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Very Rare", value: "Very Rare", color: "hsl(279, 95%, 90%)"}
      - { label: "Uncommon", value: "Uncommon", color: "hsl(330, 95%, 90%)"}
      - { label: "Legendary", value: "Legendary", color: "hsl(350, 95%, 90%)"}
      - { label: "Rare", value: "Rare", color: "hsl(303, 95%, 90%)"}
      - { label: "Artifact", value: "Artifact", color: "hsl(58, 95%, 90%)"}
      - { label: "Common", value: "Common", color: "hsl(109, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Owner:
    input: select
    accessorKey: Owner
    key: Owner
    id: Owner
    label: Owner
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 201
    options:
      - { label: "Evan Escence", value: "Evan Escence", color: "hsl(326, 95%, 90%)"}
      - { label: "Ronpip Thimble-bimble", value: "Ronpip Thimble-bimble", color: "hsl(241, 95%, 90%)"}
      - { label: "Vimack Badger", value: "Vimack Badger", color: "hsl(70, 95%, 90%)"}
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
    id: NoteIcone
    label: NoteIcon
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Item", value: "Item", color: "hsl(263, 95%, 90%)"}
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
  QuickNotes:
    input: text
    accessorKey: QuickNotes
    key: QuickNotes
    id: QuickNotes
    label: QuickNotes
    position: 100
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
  current_row_template: 
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