CLASS lcl_implement_bp_field_save IMPLEMENTATION.
  METHOD if_ex_badi_bp_field_save~before_save.
    DATA: lt_changed_fields TYPE STANDARD TABLE OF crmt_bp_fld_value,
          ls_changed_field  TYPE crmt_bp_fld_value.
    FIELD-SYMBOLS: <fs_changed_field> LIKE LINE OF lt_changed_fields.

    lt_changed_fields = ct_changed_fields.
    LOOP AT lt_changed_fields ASSIGNING <fs_changed_field>.
      WRITE: / 'Field Name:', <fs_changed_field>-field_name,
             / 'Old Value:', <fs_changed_field>-field_value_old,
             / 'New Value:', <fs_changed_field>-field_value_new.
    ENDLOOP.
  ENDMETHOD.
ENDCLASS.
