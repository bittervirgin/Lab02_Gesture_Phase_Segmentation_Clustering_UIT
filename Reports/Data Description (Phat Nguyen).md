<h1>Phân tích bộ data Gesture</h1> <br>
<br>
<h2>Chia ra làm 2 phần:</h2><br>
	<h3>Raw files VD(A1_raw):</h3><br>
		Chứa các đặc trưng vị trí của các bộ phận cơ thể tong không gian 3 chiều (x,y,z)<br>
		lh (left hand)<br>
		rh (right hand)<br>
		h (head)<br>
		s (spine)<br>
		lw (left wrist)<br>
		rw (right wrist)<br>
		timestamp<br>
		phase (output)<br>
			-- Rest<br>
			-- Preparation<br>
			-- Stroke<br>
			-- Hold<br>
			-- Retraction<br>
	<h3>Process files</h3><br>
		Chứa các vector chuyển động (hướng) của các bộ phận trên cơ thể <br>
			Các nhãn dán được đánh số từ 1 => 12<br>
				1,2,3 là vector chuyển động(VCD) của left hand<br> 
				4,5,6 là VCD của right hand<br>
				7,8,9 là VCD của left wirst<br>
				10,11,12 là VCD của right wirst<br>
		Chứa các vector gia tốc của các bộ phận trên cơ thể<br>
			Các nhãn được đánh số từ 13 => 24<br>
				12,13,14 là Vector gia tốc(VGT) của left hand<br>
				15,16,17 là VGT của right hand<br>
				18,19,20 là VGT của left wirst<br>
				21,22,23 law vgt của right wirst<br>
		Chứa các vận tốc vô hướng của các vector<br>
			các nhãn được đánh số từ 25 => 32<br>
				Có sự lặp lại ở các thuộc tính (Data Description)<br>
					25,29 là VTVH của left hand<br>
					26,30 là VTVH của right hand<br>
					27,31 là VTVH của left wirst<br>
					28,32 là VTVH cuae right wirst<br>
		phase (output)<br>
			--(R) Rest<br>
			--(P) Preparation<br>
			--(S) Stroke<br>
			--(H) Hold<br>
			--(R) Retraction<br>

<h2>*Đánh giá:</h3><br>
 	Bộ data raw files là 1 bộ dữ liệu dược xây dựng để xác trạng thái người dựa trên các tọa độ vị trí, hướng, vận tốc của các bộ phận <br> 	
