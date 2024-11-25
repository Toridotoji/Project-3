# Phân Tích Phân Khúc Khách Hàng Chiến Dịch Marketing Của IFood (2012-2014)

## Mục lục

- [Tổng quan dự án](#tổng-quan-dự-án)
- [Mục tiêu](#mục-tiêu)
- [Dữ liệu](#dữ-liệu)
- [Phương pháp phân tích dữ liệu](#phương-pháp-phân-tích-dữ-liệu)
- [Insights](#insights)

### Tổng quan dự án

IFood là nền tảng đặt đồ ăn online hàng đầu tại Brazil và phục vụ gần một triệu hành khách một năm. Danh mục sản phẩm của iFood đa dạng, bao gồm: rượu, các sản phẩm làm từ thịt, trái cây, cá và đồ ngọt. Khách hàng có thể đặt hàng thông qua 3 kênh: cửa hàng vật lý, catalog và website của công ty. Xét ở phương diện toàn cầu, iFood có lượng doanh thu ổn định trong suốt 3 năm qua, tuy nhiên, tăng trưởng lợi nhuận trong 3 năm tới không có nhiều kì vọng. Vậy nên, dự án này sẽ nhằm cải thiện hiệu quả các hoạt động marketing, bằng cách phân tích dữ liệu từ các chiến dịch trong quá khứ và xác định chiến lược phù hợp cho các chiến dịch trong tương lai.

Chiến dịch thứ 6 (sắp tới) của iFood hướng đến việc ra mắt sản phẩm mới. 1 cuộc khảo sát đã được tiến hành trên 2.240 khách hàng thông qua điện thoại. 

IFood is the lead food delivery app in Brazil, present in over a thousand cities.
Consider a well-established company operating in the retail food sector. Presently they have around several hundred thousands of registered customers and serve almost one million consumers a year. They sell products from 5 major categories: wines, rare meat products, exotic fruits, specially prepared fish and sweet products. These can further be divided into gold and regular products. The customers can order and acquire products through 3 sales channels: physical stores, catalogs and company's website. Globally, the company had solid revenues and a healthy bottom line in the past 3 years, but the profit growth perspectives for the next 3 years are not promising... For this reason, several strategic initiatives are being considered to invert this situation. One is to improve the performance of marketing activities, with a special focus on marketing campaigns.

The purpose of this project is to optimize marketing campaigns by analyzing past campaign data, identifying successful strategies, and predicting the success of future campaigns.

The objective of the team is to build a predictive model that will produce the highest profit for the next direct marketing campaign, scheduled for the next month. The new campaign, sixth, aims at selling a new gadget to the Customer Database. To build the model, a pilot campaign involving 2.240 customers was carried out. The customers were selected at random and contacted by phone regarding the acquisition of the gadget. During the following months, customers who bought the offer were properly labeled. The total cost of the sample campaign was 6.720MU and the revenue generated by the customers who accepted the offer was 3.674MU. Globally the campaign had a profit of -3.046MU. The success rate of the campaign was 15%. The objective is of the team is to develop a model that predicts customer behavior and to apply it to the rest of the customer base. Hopefully the model will allow the company to cherry pick the customers that are most likely to purchase the offer while leaving out the non-respondents, making the next campaign highly profitable. Moreover, other than maximizing the profit of the campaign, the CMO is interested in understanding to study the characteristic features of those customers who are willing to buy the gadget.

### Mục tiêu

Mục tiêu của dự án là phân tích đặc điểm hành vi khách hàng sẵn sàng mua sản phẩm mới.

Mục tiêu cụ thể được giải đáp thông qua những câu hỏi sau:
- Những chiến dịch trước đó có sự khác biệt nhiều về khách hàng so với chiến dịch thứ 6 không?
- Đặc điểm về nhân khẩu học và hành vi của tệp khách hàng tiềm năng là gì?

### Dữ liệu

Dữ liệu được cung cấp bởi công ty iFood, bao gồm các nội dung sau:
- Số lượng chiến dịch thành công
- Thông tin nhân khẩu học về khách hàng: thu nhập, giới tính... và hành vi mua như lần mua gần đây nhất, số lượt ghé trang web 1 tháng...
- Thông tin về số lượng sản phẩm được bán:

### Phương pháp phân tích dữ liệu

Xem thêm tại file [xử lý và phân tích dữ liệu](https://github.com/nhungnguyen1111/Customer_Segmentation_Analysis/blob/256484406c697dba8c071bc9d92e887fd8a3fdd9/data%20transforming%20%26%20data%20analysis.md)

### Insights 

Qua phân tích tệp khách hàng phản hồi ở chiến dịch cuối (tỷ lệ phản hồi là 14,93%), rút ra đặc điểm về khách hàng mục tiêu như sau. Đặc điểm phân tích từ last campaign không có khác biệt với 2 chiến dịch thứ 4 và thứ 3 (với tỷ lệ thành công lần lượt là 7,47% và 7,29%). Như vậy, đặc điểm về nhân khẩu học của khách hàng sẽ được rút ra từ phân tích dựa trên chiến dịch thứ 6.

![](https://i.imgur.com/F1AirQg.png)

#### Nhân khẩu học
- Tập trung vào nhóm khách hàng có độ tuổi từ 25 đến 64 tuổi
- Đây cũng là nhóm có mức thu nhập trung bình dưới R$ 63.192,19
- Những người đã kết hôn, dưới 2 con
- Có hiểu biết về sản phẩm (có học vấn từ đại học trở lên)

![](https://i.imgur.com/ck3f4ac.png)

#### Hành vi
- Mua sắm vào cửa hàng vật lý, mặc dù không có chênh lệch nhiều số lượng giao dịch mua sắm ở 3 nền tảng: cửa hàng vật lý, catalog và website
- Tổng hợp dữ liệu từ 5 chiến dịch trước cho thấy 3 nhóm KH chiếm tỷ lệ cao lần lượt là: Champion (23,16%), Can't Lose Them (22,57%) và Potential Loyalist (21,37%). Những nhóm còn lại đều dưới 12%.
  Trong giai đoạn ngắn hạn, cần tập trung vào 3 nhóm này trước và dài hạn sẽ thiết lập chiến lược cho từng nhóm khách hàng.

![](https://i.imgur.com/8i0idHJ.png)


![](https://i.imgur.com/Ngoynz7.png)

Tổng hợp chân dung khách hàng
