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
    width: 100
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  PartyStanding:
    input: select
    accessorKey: PartyStanding
    key: PartyStanding
    id: PartyStanding
    label: PartyStanding
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Dangerous", value: "Dangerous", color: "hsl(290, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Pronounced:
    input: text
    accessorKey: Pronounced
    key: Pronounced
    id: Pronounced
    label: Pronounced
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
  Ancestry:
    input: select
    accessorKey: Ancestry
    key: Ancestry
    id: Ancestry
    label: Ancestry
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Material Plane", value: "Material Plane", color: "hsl(243, 95%, 90%)"}
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
  Gender:
    input: select
    accessorKey: Gender
    key: Gender
    id: Gender
    label: Gender
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Unknown", value: "Unknown", color: "hsl(335, 95%, 90%)"}
      - { label: "Male", value: "Male", color: "hsl(99, 95%, 90%)"}
      - { label: "None", value: "None", color: "hsl(327, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Size:
    input: select
    accessorKey: Size
    key: Size
    id: Size
    label: Size
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Medium", value: "Medium", color: "hsl(81, 95%, 90%)"}
      - { label: "Large", value: "Large", color: "hsl(310, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Alignment:
    input: tags
    accessorKey: Alignment
    key: Alignment
    id: Alignment
    label: Alignment
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "NE", value: "NE", color: "hsl(301, 95%, 90%)"}
      - { label: "TN", value: "TN", color: "hsl(21, 95%, 90%)"}
      - { label: "Evil", value: "Evil", color: "hsl(274, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Condition:
    input: select
    accessorKey: Condition
    key: Condition
    id: Condition
    label: Condition
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Alive", value: "Alive", color: "hsl(165, 95%, 90%)"}
      - { label: "Dead", value: "Dead", color: "hsl(155, 95%, 90%)"}
      - { label: "Destroyed", value: "Destroyed", color: "hsl(10, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Alias:
    input: text
    accessorKey: Alias
    key: Alias
    id: Alias
    label: Alias
    position: 10
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
  Subtype:
    input: tags
    accessorKey: Subtype
    key: Subtype
    id: Subtype
    label: Subtype
    position: 11
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Aberration", value: "Aberration", color: "hsl(217, 95%, 90%)"}
      - { label: "Beast", value: "Beast", color: "hsl(124, 95%, 90%)"}
      - { label: "Dragon", value: "Dragon", color: "hsl(26, 95%, 90%)"}
      - { label: "Undead", value: "Undead", color: "hsl(69, 95%, 90%)"}
      - { label: "Slime", value: "Slime", color: "hsl(180, 95%, 90%)"}
      - { label: "Construct", value: "Construct", color: "hsl(343, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  AssociateGroup:
    input: select
    accessorKey: AssociateGroup
    key: AssociateGroup
    id: AssociateGroup
    label: AssociateGroup
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "High Elven", value: "High Elven", color: "hsl(218, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  AssociatedReligion:
    input: select
    accessorKey: AssociatedReligion
    key: AssociatedReligion
    id: AssociatedReligion
    label: AssociatedReligion
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  location:
    input: select
    accessorKey: location
    key: location
    id: location
    label: location
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Massarnae", value: "Massarnae", color: "hsl(21, 95%, 90%)"}
      - { label: "Dragon's Head", value: "Dragon's Head", color: "hsl(2, 95%, 90%)"}
      - { label: "Mira Esmirelda", value: "Mira Esmirelda", color: "hsl(113, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  Vore:
    input: select
    accessorKey: Vore
    key: Vore
    id: Diet
    label: Diet
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Unknown", value: "Unknown", color: "hsl(9, 95%, 90%)"}
      - { label: "Carnivore", value: "Carnivore", color: "hsl(182, 95%, 90%)"}
      - { label: "None", value: "None", color: "hsl(215, 95%, 90%)"}
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
  Art:
    input: text
    accessorKey: Art
    key: Art
    id: newColumn14
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