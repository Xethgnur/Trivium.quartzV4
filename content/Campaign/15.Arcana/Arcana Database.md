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
  level:
    input: select
    key: level
    accessorKey: level
    label: level
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "1st", value: "1st", color: "hsl(179, 95%, 90%)"}
      - { label: "2nd", value: "2nd", color: "hsl(221, 95%, 90%)"}
      - { label: "Unknown", value: "Unknown", color: "hsl(138, 95%, 90%)"}
      - { label: "Cantrip", value: "Cantrip", color: "hsl(186, 95%, 90%)"}
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
  castTime:
    input: select
    accessorKey: castTime
    key: castTime
    id: castTime
    label: castTime
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "1 Action", value: "1 Action", color: "hsl(160, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  range:
    input: text
    accessorKey: range
    key: range
    id: range
    label: range
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
  components:
    input: tags
    accessorKey: components
    key: components
    id: components
    label: components
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "V", value: "V", color: "hsl(263, 95%, 90%)"}
      - { label: "S", value: "S", color: "hsl(278, 95%, 90%)"}
      - { label: "/m", value: "/m", color: "hsl(48, 95%, 90%)"}
      - { label: "M", value: "M", color: "hsl(33, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  duration:
    input: tags
    accessorKey: duration
    key: duration
    id: duration
    label: duration
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Concentration", value: "Concentration", color: "hsl(212, 95%, 90%)"}
      - { label: "10 minutes", value: "10 minutes", color: "hsl(177, 95%, 90%)"}
      - { label: "PT10M", value: "PT10M", color: "hsl(339, 95%, 90%)"}
      - { label: "1 Round", value: "1 Round", color: "hsl(221, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  school:
    input: select
    accessorKey: school
    key: school
    id: school
    label: school
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Divination", value: "Divination", color: "hsl(314, 95%, 90%)"}
      - { label: "Enchantment", value: "Enchantment", color: "hsl(123, 95%, 90%)"}
      - { label: "Evocation", value: "Evocation", color: "hsl(170, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  attack:
    input: text
    accessorKey: attack
    key: attack
    id: attack
    label: attack
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
  damage:
    input: select
    accessorKey: damage
    key: damage
    id: damage
    label: damage
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Control", value: "Control", color: "hsl(284, 95%, 90%)"}
      - { label: "Radiant", value: "Radiant", color: "hsl(178, 95%, 90%)"}
      - { label: "Thunder", value: "Thunder", color: "hsl(248, 95%, 90%)"}
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