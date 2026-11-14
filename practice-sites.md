# Practice sites for portfolio samples

All links checked and working on 2026-11-15.

## Which site for which sample

| Sample | Site | Link |
|---|---|---|
| Bug reports | Toolshop (with planted bugs) | https://with-bugs.practicesoftwaretesting.com |
| Test cases | Toolshop (normal version) | https://practicesoftwaretesting.com |
| Playwright | Sauce Demo (already using) | https://www.saucedemo.com |
| Postman collection | Restful-Booker | https://restful-booker.herokuapp.com |

## All links

### Toolshop (Practice Software Testing)
- Normal site: https://practicesoftwaretesting.com
- Version with bugs: https://with-bugs.practicesoftwaretesting.com
- API: https://api.practicesoftwaretesting.com/products
- Has: login, search, filters, cart, checkout, invoices.
- Use for: test cases (checkout flow) and bug reports (one functional, one UX).

### Restful-Booker
- API: https://restful-booker.herokuapp.com/booking
- Docs: https://restful-booker.herokuapp.com/apidoc/index.html
- Has: auth token, create / read / update / delete bookings, some planted bugs.
- Use for: Postman collection with a create → read → update → delete chain that passes the token between requests.

### Restful-Booker Platform (B&B site)
- Site: https://automationintesting.online
- Has: room booking, contact form, admin panel.
- Use for: a UX bug report (confusing flows, weak error messages).

### Automation Exercise
- Site: https://automationexercise.com
- API list: https://automationexercise.com/api_list
- Use for: backup option that covers both UI and API on one site.

### ParaBank
- Site: https://parabank.parasoft.com/parabank/index.htm
- Has: transfers, bill pay, loans.
- Use for: banking samples, if you want something other than e-commerce.

## Sample checklist

- [ ] Bug report 1: functional bug, with screenshot or recording
- [ ] Bug report 2: UX bug, with screenshot or recording
- [ ] Test cases: one-paragraph requirement + 10 to 15 cases (include negative and edge cases)
- [ ] Playwright repo: 5 to 10 tests, README, passing GitHub Actions run
- [ ] Postman collection: exported JSON + short README

In each write-up, say that it's a practice site built for testers.
