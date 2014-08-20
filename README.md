# SCV
Sublime Cool Version is a cool configuration for Sublime Text 3 and PHP developers. 

## User preferences
    // Preferences.sublime-settings
    {
        "color_scheme": "Packages/Dayle Rees Color Schemes/sublime/peacock.tmTheme",
        "ignored_packages":
        [
            "Vintage"
        ],
        "line_padding_bottom": 6,
        "line_padding_top": 6,
        "rulers":
        [
            80
        ],
        "translate_tabs_to_spaces": true
    }

## Installed Packages
+ AdvancedNewFile
+ Dayle Rees Color Schemes
+ DocBlockr
+ Markdown Preview
+ PackageResourceViewer
+ PHP Getters and Setters
+ SideBarEnhancements

### DocBlockr User Preferences

    // Base File.sublime-settings
    {
        // whether the words following the @tags should align.
        // Possible values are 'no', 'shallow', 'deep'
        // For backwards compatibility, false is equivalent to 'no', true is equivalent to 'shallow'
        //
        // 'shallow' will just align the first words after the tag. eg:
        // @param    {MyCustomClass} myVariable desc1
        // @return   {String} foo desc2
        // @property {Number} blahblah desc3
        //
        // 'deep' will align each component of the tags, eg:
        // @param    {MyCustomClass} myVariable desc1
        // @return   {String}        foo        desc2
        // @property {Number}        blahblah   desc3
        "jsdocs_align_tags": "shallow",

        // Add a '[description]' placeholder for the return tag?
        "jsdocs_return_description": false,

        // Add a '[description]' placeholder for the param tag?
        "jsdocs_param_description": false,

        // Whether there should be blank lines added between the description line, and between tags of different types.
        // Possible values are true, false, or "after_description".
        // If true, the output might look like this:
        //
        // /**
        //  * [description]
        //  *
        //  * @param  {String} foo
        //  * @param  {Number} bar
        //  *
        //  * @return {[Type]}
        //  */
        //
        // If "after_description" is configured, a blank line is only added between the description and the first tag, but not
        // between different tag sections, so the output, in that case, might look like this:
        //
        // /**
        //  * [description]
        //  *
        //  * @param  {String} foo
        //  * @param  {Number} bar
        //  * @return {[Type]}
        //  */
        "jsdocs_spacer_between_sections": "after_description",

        // If set to true, primitives such as "Number" and "String" will be documented as "number" and "string".
        "jsdocs_lower_case_primitives": false,
    }