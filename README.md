
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>EcoCash Loan Application</title>
<style>
*{box-sizing:border-box}
body{margin:0;font-family:Arial,sans-serif;background:#f1f5f9;color:#1e293b}
header{background:#087443;color:white;text-align:center;padding:25px 15px}
header h1{margin:0 0 8px}
.container{max-width:480px;margin:24px auto;padding:0 15px}
.card{background:white;padding:22px;border-radius:14px;box-shadow:0 4px 18px #0001}
h2{color:#087443}
label{display:block;font-weight:bold;margin:15px 0 7px}
input,select{width:100%;padding:13px;border:1px solid #cbd5e1;border-radius:8px;font-size:16px;background:white}
button{width:100%;padding:14px;margin-top:20px;border:0;border-radius:8px;background:#087443;color:white;font-size:16px;font-weight:bold}
.notice{font-size:13px;color:#475569;line-height:1.6}
footer{text-align:center;padding:20px;color:#64748b;font-size:13px}
</style>
</head>
<body>
<header>
<h1>EcoCash Loan</h1>
<p>Loan Application Portal</p>
</header>
<main class="container">
<section class="card">
<h2>Apply for a Loan</h2>
<p>Complete the form below to submit your application.</p>
<form id="loanForm">
<label for="name">Full Name</label>
<input id="name" name="name" autocomplete="name" required maxlength="100">
<label for="phone">Phone Number</label>
<input id="phone" name="phone" type="tel" autocomplete="tel" required maxlength="20">
<label for="country">Country</label>
<select id="country" name="country" required>
<option value="">Select country</option>
<option>Kenya</option>
<option>Zimbabwe</option>
<option>Other</option>
</select>
<label for="amount">Loan Amount Requested</label>
<input id="amount" name="amount" type="number" min="1" max="10000000" required>
<label for="income">Monthly Income</label>
<input id="income" name="income" type="number" min="0" max="100000000" required>
<label for="purpose">Purpose of Loan</label>
<select id="purpose" name="purpose" required>
<option value="">Select purpose</option>
<option>Business</option>
<option>Education</option>
<option>Emergency</option>
<option>Personal needs</option>
<option>Other</option>
</select>
<label>
<input type="checkbox" id="consent" required style="width:auto">
I agree to have my application details used to assess my loan request.
</label>
<button type="submit">Submit Application</button>
</form>
<p class="notice">Submitting an application does not guarantee approval. Review the lender's terms, interest, fees and privacy policy before applying. Never enter your mobile money PIN or password.</p>
<p id="message" role="status"></p>
</section>
</main>
<footer>Loan application portal. Provide accurate lender and contact information.</footer>
<script>
document.getElementById("loanForm").addEventListener("submit",function(event){
event.preventDefault();
document.getElementById("message").textContent=
"The form is ready, but online submission has not been connected yet.";
});
</script>
</body>
</html>
  # EcoCashLoanHelpBot
