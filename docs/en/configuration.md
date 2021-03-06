# Configuration

- [Basic Configuration](#basic)
- [Extra Configuration](#extra)

<hr>

Below is the full configuration available with defaults.

    protected $fields = [
        "example" => [
            "type"   => "anomaly.field_type.country",
            "config" => [
                "default_value" => null,
                "separator" => ",",
                "point"     => ".",
                "decimals"  => 2,
                "min"       => 0
            ]
        ]
    ];

<hr>

<a name="basic"></a>
## Basic Configuration

### Default Value

    "default_type" => 25.00

The `default_value` is a core option. This field type accepts any decimal value. The value will be converted into the configured format automatically.

<hr>

<a name="extra"></a>
## Extra Configuration

### Thousands Separator

    "separator" => ","

Specify the thousands separator character to use for input / output. Any valid character can be specified.

### Decimal Point

    "point" => "."

Specify the decimal point character to use for input / output. Any valid character can be specified.

### Decimal Places

    "decimals" => 4

Specify the number of decimal places to use for input / output.

<div class="alert alert-primary">
<strong>Note:</strong> This option determines storage format and can not be set dynamically on the form builder.
</div>