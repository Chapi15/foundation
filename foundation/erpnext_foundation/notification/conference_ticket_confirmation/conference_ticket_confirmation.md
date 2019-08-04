<p>Dear {{ doc.participant_name }},</p>

<p>Thank you for registering for the 2019 ERPNext Conference!</p>

<p>Here are your ticket details:</p>

<h4>Ticket Number {{ doc.name}}</h4>

<table class="table table-bordered" border="0" cellpadding="0" cellspacing="0" width="100%" style="padding: 30px 0px">
	<tr>
		<th style='width: 50%'>Ticket Type</th>
		<th style='width: 25%'>Qty</th>
		<th style='width: 25%'>Rate</th>
	</tr>
	<tr>
		<td>Conference Tickets + Lunch + Dinner</td>
		<td>{{ doc.full_conference_tickets or 0 }}</td>
		<td>{% if doc.currency=="INR" %}5000{% else %}70{% endif %}</td>
	</tr>
</table>

<h5>Total Amount: {{ doc.currency }} {{ doc.get_formatted('amount') }}</h5>


<p>If you need any help, please email us at foundation@erpnext.com</p>