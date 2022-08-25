# Liquid Programming

## A Tamplating Language

<hr>

[Link](URL)

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

### **Operator**

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

### **if else condition**

```bash
{% if your_condition %}
{% else if your_condition %}
{% else your_condition %}
{% endif %}
```

> Examples:
> <br> {% if num1 > num2 %} <br> Grater number is {{ num1 }} <br>{% elsif num1 < num2  %} <br>Grater number is {{ num2 }} <br> {% else num1 == num2 %} <br> Both are equal <br> {% endif %} <br>
