# `validateForm(options)`

## Options

<table>
  <thead>
    <th>Option</th>
    <th>Description</th>
  </thead>
  <tbody>
    <tr>
      <td>
        formData
      </td>
      <td>
        The form data to validate. In the form of:
<pre>{
  [fieldName]: {
    value: [value],
    rules: [rules], // E.g "required|image"
  }
}</pre>
      </td>
    </tr>
    <tr>
      <td>
        includeMessages
      </td>
      <td>
        `errors[field]` will be a message instead of rule name (Currently default messages are rule name)
      </td>
    </tr>
  </tbody>
</table>

## Return value

```
{
  [fieldName]: [rule|message],
  ...
}
```