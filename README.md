# Liquid Programming

## A Tamplating Language

<hr>

[Liquid Documentation](https://shopify.github.io/liquid/)

### **Start End Condition**

```bash
{% %}
```

### **Output print**

```bash
{{ }}
```

### **Variable Declear**

```bash
{{ assign variable_name = variable_value }}
```

> Examples:
> <br> {{ assign myName = "Shama" }}

### **Comment**

```bash
{% comment %}
    your_text
{% endcomment %}
```

> Examples:
> <br> {% comment %}
> My name is shama
> {% endcomment %}

### **Mathmatical Operators**

```bash
Asisgn Operator- =
Add Operator- | plus:
Substraction Operator- | minus:
Multiplication Operator- | times:
Division Operator- | divided_by:
Modulas Operator- | modulo:
```

> Examples:
> <br> Assignment Operator
> <br> ---------------------
> <br> {%  assign num1 = 10 %} <br> {%  assign num2 = 4 %} <br><br> Addition: {{ num1 | plus: num2 }}<br> Substraction: {{ num1 | minus: num2 }}<br> Multipication: {{ num1 | times: num2 }}<br> Division: {{ num1 | divided_by: num2 }}<br> Modulas: {{ num1 | modulo: num2 }}<br>

### **Conditional Operators**

```bash
Equal Operator- ==
Graterthen operator- >
Graterthen or equal operator- >=
Lessthen Operator- <
Lessthen or equal Operator- <=
And operator- and
Or operator- or

```

> Examples:
> <br> {% if num1 > num2 and num1 > num3 %} <br> Grater number is {{ num1 }} <br> {% else %} <br> {{ num1 }} is not grater number <br> {% endif %} <br>

### **if else condition**

```bash
{% if your_condition %}
        Your_Output
    {% elsif your_condition %}
        Your_Output
    {% else your_condition %}
        Your_Output
{% endif %}
```

> Examples:
> <br> {% if num1 > num2 %} <br> Grater number is {{ num1 }} <br>{% elsif num1 < num2  %} <br>Grater number is {{ num2 }} <br> {% else num1 == num2 %} <br> Both are equal <br> {% endif %} <br>

### **Switch Case**

```bash
{% case your_input %}
    {% when your_condition %}
        Your_Output
    {% when your_condition %}
        Your_Output
    {% when your_condition %}
        Your_Output
    {% else %}
        Your_Output
{% endcase %}
```

> Examples:
> <br>{% assign color= "black" %}<br><br> {% case color %} <br> {% when "red" %} <br> Color is {{ color }} <br> {% when "green" %} <br> Color is {{ color }} <br> {% when "blue" %} <br> Color is {{ color }} <br> {% else %} <br> Your color is not listed <br> {% endcase %}

### **For Loop**

```bash
{% for vatiable_name in your_input %}
    {{ vatiable_name }}
{% endfor %}
```

> Examples:
> <br> {% for item in (1..6) %}<br> {{ item }} <br> {% endfor %}<br>
