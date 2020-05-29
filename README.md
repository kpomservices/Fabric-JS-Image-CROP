# Fabric-JS-Image-CROP
Image Cropping in Fabric JS

Demo:
http://kpomservices.com/imagecropdemo/index.html

Actions:
Double Click on the image to crop,
Click outside the image to complete the crop.

Changes needed in fabric js 
Function to change in fabric js library:
	_renderFill: function(ctx)

Change

          sX = Math.max(0, this.cropX * this._filterScalingX),
          sY = Math.max(0, this.cropY * this._filterScalingY);

To

          sX = this.cropX * this._filterScalingX,
          sY = this.cropY * this._filterScalingY;
