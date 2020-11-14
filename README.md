

{% block body %}
<div class="jumbotron">
    <h2 style="text-align: center; color: #206aaa;">Sign Up Form</h2>
    {% from "includes/_formhelpers.html" import render_field %}
    <form method="POST" action="">
        <div class="form-group">
            {{render_field(form.name, class_="form-control")}}
        </div>
        <div class="form-group">
            {{render_field(form.email, class="form-control")}}
        </div>
        <div class="form-group">
            {{render_field(form.username, class="form-control")}}
        </div>
        <div class="form-group">
            {{render_field(form.password, class="form-control")}}
        </div>
        <p>
            <input type="submit" class="btn btn-primary" value="Sign Up">
        </p>
    </form>
</div>
{% endblock %}
