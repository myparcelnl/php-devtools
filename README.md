# MyParcel PHP DevTools

These tools are used to make a consistent php workflow.

## Installation

```bash
composer require --dev myparcelnl/devtools
```

## Included tools

- [PHPMD](#PHPMD)

## Configuration

### PHPMD

Create a new file in your project root called `phpmd.xml`.

Paste the following content into it:

```xml
<?xml version="1.0"?>
<ruleset xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         name="MyParcel"
         xmlns="http://pmd.sf.net/ruleset/1.0.0"
         xsi:schemaLocation="http://pmd.sf.net/ruleset/1.0.0 https://pmd.sourceforge.io/ruleset_xml_schema.xsd"
         xsi:noNamespaceSchemaLocation="https://pmd.sourceforge.io/ruleset_xml_schema.xsd">
    <description />

    <rule ref="vendor/myparcelnl/devtools/phpmd.xml">
        <exclude name="StaticAccess" />
    </rule>
</ruleset>
```

Then set up your IDE so PHPMD inspections are enabled.
