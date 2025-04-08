<!--


{% extends 'todo/base.html' %}

{% block content %}
<h1>To-Do List</h1>
<form action="{% url 'add_todo' %}" method="POST">
  {% csrf_token %}
  <input type="text" name="title" placeholder="Enter a new task">
  <button type="submit">Add</button>
</form>

<ul>
  {% for todo in todos %}
  <li>
      <span class="{% if todo.completed %}completed{% else %}not-completed{% endif %}">
          {{ todo.title }}
      </span>
      <a href="{% url 'update_todo' todo.id %}">Toggle</a>
      <a href="{% url 'delete_todo' todo.id %}">Delete</a>
  </li>
  {% endfor %}
</ul>
{% endblock %}

-->

