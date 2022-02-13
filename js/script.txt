 if(!config.showScrollMsg){
            frames[0].style.display = "flex";
            setTimeout(() => {
                frames[0].classList.add("appear");
                frames[0].style.opacity = "1";
            }, 1500);
            return;
        }

        document.querySelector(".HBD").textContent = "May your soul rest in peace";

        frames[1].style.display = "flex";

        setTimeout(() => {
            frames[1].classList.add("appear");
            frames[1].style.opacity = "1";
            msg.classList.add("move-up");
        },1500);

        setTimeout(() => {
            msg.style.transform = "translateY(-100%)";
            flash.style.display = "none";
        },5000);

        setTimeout(() => {
            msgWindow.classList.add("fade-in");
            msgWindow.style.opacity = '0';
        },88000);

        setTimeout(() => {
            frames[1].style.display = "none";
            frames[0].style.display = "flex";
            frames[0].classList.add("appear");
            frames[0].style.opacity = "1";
        },91000);

    }

});