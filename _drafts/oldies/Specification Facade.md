Вот есть спецификация на Hermes.

Там буквально описывается 3 формата файлов: 2 генерировать 1 парсить. А потом к 1 одному файлу "запросы". Каждый запрос - отдельная секция в спецификации.

Как строить разработку? Должна ли внутренняя реализация кода по спецификации структурно совпадать с самой спецификацией или эти подробности должны раствориться в клиентском коде каким-то более оптимальным образом? (другими словами, будет ли клиент драйвтиь методы API или наоборот? Может какие-то запросы из спецификации стоит растворить скомбинировать?)

Specification Facade - хорошее название паттерна. По сути, просто разновидность фасада. Что дает: всегда легко проверить соответствие бумажной спецификации ее реализации. Структура тестов покрывает разделы спецификации. Как правило к спецификациям форматов в комплекте еще идут гайды, которые будут документацией к вашему апи.

Минусы: избыточность, неоптимальность клиентского кода.