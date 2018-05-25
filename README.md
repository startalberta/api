# API documentation
API documention and examples

## Authentification

No authentification is required at the moment.

## Rate limiting

A maximum of <span class="tag">5 requests per minut</span> is allowed.

## Getting started

All requests are made on <span class="tag">https://startalberta.com/api/</span> via GET requests and url parameters.

## Entities

<table>

<thead>

<tr>

<th>Entity</th>

<th>Url</th>

</tr>

</thead>

<tbody>

<tr>

<td>Article</td>

<td>articles</td>

</tr>

<tr>

<td>Company</td>

<td>companies</td>

</tr>

<tr>

<td>Event</td>

<td>events</td>

</tr>

<tr>

<td>Individual</td>

<td>individuals</td>

</tr>

<tr>

<td>Investment</td>

<td>investments</td>

</tr>

<tr>

<td>Investor</td>

<td>investors</td>

</tr>

<tr>

<td>Job</td>

<td>jobs</td>

</tr>

<tr>

<td>Organization</td>

<td>organization</td>

</tr>

<tr>

<td>Program</td>

<td>program</td>

</tr>

<tr>

<td>Vc Firm</td>

<td>vc-firm</td>

</tr>

</tbody>

</table>

For example, this is the request to retrieve all companies

<pre>GET https://startalberta.com/api/companies</pre>

## Pagination

All responses are paginated, change page via the <span class="tag">page</span> parameter

<pre>GET https://startalberta.com/api/companies?page=2</pre>

## Search

You can search on all the fields of an entity with the <span class="tag">search</span> parameter.

<pre>GET https://startalberta.com/api/companies?search=Acme</pre>

## Filter

You can filter on specific fields of an entity.

<pre>GET https://startalberta.com/api/companies?name=Acme&created_at=2018-01-01&stage=Validating</pre>

This will search all companies containing 'Acme' in their name, created on 2018-01-01 and having the 'Validating' stage.

## Sort

You can sort on specific fields of an entity with the <span class="tag">sort_field</span> and <span class="tag">sort_order</span> parameters.

<pre>GET https://startalberta.com/api/companies?sort_field=id&sort_order=desc</pre>

## Bug or issues?

Please report it on [GitHub](https://github.com/startalberta/api)
