<!DOCTYPE html>
<html>
<head>
	<title>Jam Analog </title>
	<script src="ttttttt"></script>
</head>
<body>
	<style type="text/css">
	body {

background-image : url("zero two.jpg");


}

	h1,h2,p,a{
		font-family: sans-serif;
		font-weight: normal;
	}

	.jam_analog_malasngoding {
		background: #e7f2f7;
		position: relative;
		width: 240px;
		height: 240px;
		border: 16px solid #52b6f0;
		border-radius: 50%;
		padding: 20px;
		margin:20px auto;
	}

	.xxx {
		height: 100%;
		width: 100%;
		position: relative;
	}

	.jarum {
		position: absolute;
		width: 50%;
		background: #232323;
		top: 50%;
		transform: rotate(90deg);
		transform-origin: 100%;
		transition: all 0.05s cubic-bezier(0.1, 2.7, 0.58, 1);
	}

	.lingkaran_tengah {
		width: 24px;
		height: 24px;
		background: #232323;
		border: 4px solid #52b6f0;
		position: absolute;
		top: 50%;
		left: 50%;
		margin-left: -14px;
		margin-top: -14px;
		border-radius: 50%;
	}

	.jarum_detik {
		height: 2px;
		border-radius: 1px;
		background: #F0C952;
	}

	.jarum_menit {
		height: 4px;
		border-radius: 4px;
	}

	.jarum_jam {
		height: 8px;
		border-radius: 4px;
		width: 35%;
		left: 15%;
	}
</style>


<center>
	<h1>JAM KONTOL</h1>
	<h2>MIFTAH_GANTENG</h2>
	<label>TULIS PENDAPAT<P><input type="text" name="field1" /></label>
</center>

<div class="jam_analog_malasngoding">
	<div class="xxx">
		<div class="jarum jarum_detik"></div>
		<div class="jarum jarum_menit"></div>
		<div class="jarum jarum_jam"></div>
		<div class="lingkaran_tengah"></div>
	</div>
</div>

<center>
	<div class="button-section"><p>
	
	<p> KLIK SUBMIT YA ANJING !!!!<p/>
	<a href="https://instagram.com/mfth.dm?igshid=YmMyMTA2M2Y=">
<input type="submit" name="Sign Up" />
</center>




<script type="text/javascript">
	const secondHand = document.querySelector('.jarum_detik');
	const minuteHand = document.querySelector('.jarum_menit');
	const jarum_jam = document.querySelector('.jarum_jam');

	function setDate(){
		const now = new Date();

		const seconds = now.getSeconds();
		const secondsDegrees = ((seconds / 60) * 360) + 90;
		secondHand.style.transform = `rotate(${secondsDegrees}deg)`;
		if (secondsDegrees === 90) {
			secondHand.style.transition = 'none';
		} else if (secondsDegrees >= 91) {
			secondHand.style.transition = 'all 0.05s cubic-bezier(0.1, 2.7, 0.58, 1)'
		}

		const minutes = now.getMinutes();
		const minutesDegrees = ((minutes / 60) * 360) + 90;
		minuteHand.style.transform = `rotate(${minutesDegrees}deg)`;

		const hours = now.getHours();
		const hoursDegrees = ((hours / 12) * 360) + 90;
		jarum_jam.style.transform = `rotate(${hoursDegrees}deg)`;
	}

	setInterval(setDate, 1000)
</script>
</body>
</html>
