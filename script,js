    /**
     * Открытие модального окна
     * Аргумент это id модалки, чтобы можно было вызывать универсально
     */
    function showModal(name_modal){
        /**
         * Получаем ссылку на модалку по ее классу.(находит первый элемент с таким классом на странице)
         */
        let modal = document.querySelector('#'+name_modal);

        /**
         * меняем значение дисплей на block
         */
        modal.style.display = 'block';

        /**
         * Получаем кнопку закрыть для этой модалки
         */
        let close = modal.querySelector('.popup-close');
        close.addEventListener('click', closeModal.bind(null, name_modal)); //передаем параметры в функцию без ее вызова
    }

    /**
     * Закрытие модального окна
     */
    function closeModal(name_modal){
        let modal = document.querySelector('#'+name_modal);
        modal.style.display = 'none';
    }

    /**
     * Обработка нажания кнопки для запуска модалки
     * param@ name_button = class buton
     */
    function btnShowModal(name_button){
        let btn = document.querySelector('.'+name_button);
        btn.addEventListener('click', clikBtnModalShow);

        function clikBtnModalShow(){
            let name_modal = this.getAttribute('data-modal');
            if(name_modal != null && name_modal.length > 0) showModal(name_modal);
        }
    }

    btnShowModal('more'); // 
