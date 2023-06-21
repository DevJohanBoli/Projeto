# TCC


.fundo_modal_form{
    font-family: "Roboto", sans-serif;
    width: 100%;
    height: 100%;
}
.fade_modal{
    display: none;
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 11;
    background-color: rgba(0, 0, 0, 0.6);
}

.modal_form{
    position: fixed;
    left: 50%;
    top: -100%;
    transform: translate(-50%, -50%) scale(1.15);
    width: calc(100% - 20px);
    max-width: 650px;
    background-color: #FFF;
    z-index: 12;
    padding: 50px 40px 40px;
    border-radius: 20px;
    display: grid;
    opacity: 0;
    gap: 10px;
    transition: top 0ms ease-in-out 300ms, 
    transform 300ms ease-in-out 0ms,
    opacity 300ms ease-in-out 0ms;
}
.modal_form.active{
    top: 50%;
    transform: translate(-50%, -50%) scale(1);
    opacity: 1;
    transition: top 0ms ease-in-out 0ms,
                transform 300ms ease-in-out 0ms,
                opacity 300ms ease-in-out 0ms;
}
.form_image{
    display: flex ;
    align-items: center;
}

.form_txt h2{
    font-size: 28px;
    font-family: "Montserrat", sans-serif;
    line-height: 1.15;
    margin-bottom: 10px;
    color: #111;
}

.form_txt p{
    font-size: 16px;
    color: #555;
    margin-bottom: 15px;
}

.inputForm label{
    display: block;
    margin-bottom: 5px;
    font-size: 15px;
}

.inputForm{
    margin-bottom: 10px;
}

.inputForm input{
    width: 100%;
    padding: 10px;
    border: 1px solid #aaa;
    font-size: 15px;
    border-radius: 5px;
}

.formulario button{
    width: 100%;
    padding: 8px;
    font-size: 15px;
    border-radius: 5px;
    border: none;
    outline: none;
    cursor: pointer;
    background: var(--roxoclaro--);
    color: #FFF;
    box-shadow: 0px 2px 2px #ddd;
}

@media (min-width:680px){
    .modal_form{
        grid-template-columns: repeat(2, 1fr);

    }
}
#closeModalForm{
    position: absolute;
    top: 10px;
    right: 10px;
    padding: 5px;
    font-size: 18px;
    cursor: pointer;
    background:transparent;
    color: #555;
    border: none;
}