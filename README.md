# zillow_transactions
solution
select city
from zillow_transactions
group by city 
having avg(mkt_price)>
(select AVG(mkt_price) from zillow_transaction)
