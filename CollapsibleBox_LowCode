$w.onReady(function () {	
	$w('#OneCollapsibleButton').onClick(() => {
		toggleBox($w('#OneCollapsibleBox'), $w('#OnePlusSing'), $w('#OneMinusSing'));
	});
	$w('#TwoCollapsibleButton').onClick(() => {
		toggleBox($w('#TwoCollapsibleBox'), $w('#TwoPlusSing'), $w('#TwoMinusSing'));
	});
	$w('#ThreeCollapsibleButton').onClick(() => {
		toggleBox($w('#ThreeCollapsibleBox'), $w('#ThreePlusSing'), $w('#ThreeMinusSing'));
	});
});

function toggleBox(boxElement, plusSign, minusSign) {
	const isCollapsed = boxElement.collapsed;
	if (isCollapsed) {
		plusSign.hide();
		minusSign.show();
		boxElement.expand();
	} else {
		minusSign.hide();
		plusSign.show();
		boxElement.collapse();
	}
}