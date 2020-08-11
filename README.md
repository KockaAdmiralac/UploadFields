# UploadFields
This is a fork of [HydraWiki's UploadFields extension](https://github.com/HydraWiki/UploadFields) with improvements I personally needed when running this extension on vanilla MediaWiki 1.34.

## Changes
- Serbian localization (only the description message).
- New configuration variables:
    - `$wgUploadFieldsParameterNamePadding`: A number, by default set to zero, that determines the amount of spaces your parameter names will have after their name.
    - `$wgUploadFieldsRemoveBlank`: Whether blank fields should be removed from template's parameters. Set to `true` by default.
    - `$wgUploadFieldsSummaryParameter`: Name of the parameter in which the summary field's text will be inserted.
    - `$wgUploadFieldsTemplate`: Name of the wiki's file description template.
- Additional spaces are added before and after parameter names, as well as after the `=` sign, regardless of the parameter name padding settings.
- Removed the previous README as it just copied the [MediaWiki.org documentation page](https://mediawiki.org/wiki/Extension:UploadFields).
- Allowed different field labels from parameter names by changing the contents of `MediaWiki:UploadFields-label-Name` pages. When these pages don't exist, messages remain the same.
- Trimming select/multiselect types/labels.
